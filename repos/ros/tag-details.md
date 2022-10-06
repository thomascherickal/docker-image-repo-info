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
$ docker pull ros@sha256:d46c1bb8761c07e3840c9e01a3f944fc554be7261b9438e2a0a24786c7c25966
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:4204c90c6b28897e40ae8897665c2cc60984a5e0bcc9beb12ebbea16fede6fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (250956849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8f7811980a3e21304d7a71567d602527b90d81b54c2009d4e16f66d92e8303`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:24:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:25:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:25:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bed5d7de950633b22457faefa5a82b47b766d96c02665e4faf86d9b7ebe9703`  
		Last Modified: Wed, 05 Oct 2022 10:55:53 GMT  
		Size: 73.3 MB (73322093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e37e53cfffae15445cfdce1b4b7ef7cea4b3e153ea7abf8cd18ebf02b77e34`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 267.4 KB (267375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b37769ea581ebd1d2e907d8c68c8a2c4f7920ce4e81e0099e4165a54aca77`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 2.4 KB (2419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216bc94919c7136aa052456840629454991399309eea61f5b2f7b34471de467c`  
		Last Modified: Wed, 05 Oct 2022 10:55:45 GMT  
		Size: 21.7 MB (21663849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:70f4a3bc45e257fba41f608f2f06358381f46476287c05ebd2acbc6a9e42d658
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226394124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cbcd1b77d057daa39433a40f5ee770ec42c38f88e2df4979685b4613fabcfc2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:50:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:50:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b933fcbe46312ae813f092369a156c253b1e52cb3a43298b9a4fdbee1eb6fa6b`  
		Last Modified: Wed, 05 Oct 2022 14:14:40 GMT  
		Size: 67.4 MB (67449275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d7c2e640d21fee0497f12b54a0f888d39799eb93389888e1da33e797737919`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 267.3 KB (267323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2d4224582edb4e076612a46599ad24ba3ccfc164b2d512b2006c21094a621`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81d9c31822b3bf7270af1ce9bc509a7516e60401dcfc80333756e3f62d45364`  
		Last Modified: Wed, 05 Oct 2022 14:14:33 GMT  
		Size: 20.4 MB (20366915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:d46c1bb8761c07e3840c9e01a3f944fc554be7261b9438e2a0a24786c7c25966
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:4204c90c6b28897e40ae8897665c2cc60984a5e0bcc9beb12ebbea16fede6fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (250956849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8f7811980a3e21304d7a71567d602527b90d81b54c2009d4e16f66d92e8303`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:24:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:25:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:25:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bed5d7de950633b22457faefa5a82b47b766d96c02665e4faf86d9b7ebe9703`  
		Last Modified: Wed, 05 Oct 2022 10:55:53 GMT  
		Size: 73.3 MB (73322093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e37e53cfffae15445cfdce1b4b7ef7cea4b3e153ea7abf8cd18ebf02b77e34`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 267.4 KB (267375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b37769ea581ebd1d2e907d8c68c8a2c4f7920ce4e81e0099e4165a54aca77`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 2.4 KB (2419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216bc94919c7136aa052456840629454991399309eea61f5b2f7b34471de467c`  
		Last Modified: Wed, 05 Oct 2022 10:55:45 GMT  
		Size: 21.7 MB (21663849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:70f4a3bc45e257fba41f608f2f06358381f46476287c05ebd2acbc6a9e42d658
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226394124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cbcd1b77d057daa39433a40f5ee770ec42c38f88e2df4979685b4613fabcfc2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:50:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:50:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b933fcbe46312ae813f092369a156c253b1e52cb3a43298b9a4fdbee1eb6fa6b`  
		Last Modified: Wed, 05 Oct 2022 14:14:40 GMT  
		Size: 67.4 MB (67449275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d7c2e640d21fee0497f12b54a0f888d39799eb93389888e1da33e797737919`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 267.3 KB (267323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2d4224582edb4e076612a46599ad24ba3ccfc164b2d512b2006c21094a621`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81d9c31822b3bf7270af1ce9bc509a7516e60401dcfc80333756e3f62d45364`  
		Last Modified: Wed, 05 Oct 2022 14:14:33 GMT  
		Size: 20.4 MB (20366915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:d46c1bb8761c07e3840c9e01a3f944fc554be7261b9438e2a0a24786c7c25966
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:4204c90c6b28897e40ae8897665c2cc60984a5e0bcc9beb12ebbea16fede6fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (250956849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8f7811980a3e21304d7a71567d602527b90d81b54c2009d4e16f66d92e8303`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:24:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:25:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:25:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bed5d7de950633b22457faefa5a82b47b766d96c02665e4faf86d9b7ebe9703`  
		Last Modified: Wed, 05 Oct 2022 10:55:53 GMT  
		Size: 73.3 MB (73322093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e37e53cfffae15445cfdce1b4b7ef7cea4b3e153ea7abf8cd18ebf02b77e34`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 267.4 KB (267375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b37769ea581ebd1d2e907d8c68c8a2c4f7920ce4e81e0099e4165a54aca77`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 2.4 KB (2419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216bc94919c7136aa052456840629454991399309eea61f5b2f7b34471de467c`  
		Last Modified: Wed, 05 Oct 2022 10:55:45 GMT  
		Size: 21.7 MB (21663849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:70f4a3bc45e257fba41f608f2f06358381f46476287c05ebd2acbc6a9e42d658
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226394124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cbcd1b77d057daa39433a40f5ee770ec42c38f88e2df4979685b4613fabcfc2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:50:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:50:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b933fcbe46312ae813f092369a156c253b1e52cb3a43298b9a4fdbee1eb6fa6b`  
		Last Modified: Wed, 05 Oct 2022 14:14:40 GMT  
		Size: 67.4 MB (67449275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d7c2e640d21fee0497f12b54a0f888d39799eb93389888e1da33e797737919`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 267.3 KB (267323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2d4224582edb4e076612a46599ad24ba3ccfc164b2d512b2006c21094a621`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81d9c31822b3bf7270af1ce9bc509a7516e60401dcfc80333756e3f62d45364`  
		Last Modified: Wed, 05 Oct 2022 14:14:33 GMT  
		Size: 20.4 MB (20366915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:23ccc9dbba22bb04efb39700e30838e421e3078a4c8020fd6a8c3a3258755585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:47bbdada6ec4dbc2f19ed702bcbd8916a26f8964a2c25790dd65668cfb939d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155701113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7ee85a49e46466a088fa050f4373b9accb131b1b137c3650e9919ecd67d036`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:52ee321733098fccaaf6a0618e45b7dc52f08ce058fb8349984592e05de6bf38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138308211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9bc639ef7ce7d698d0dce478a9a4828085c53c24246570ed03bd3b8871dc0b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:23ccc9dbba22bb04efb39700e30838e421e3078a4c8020fd6a8c3a3258755585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:47bbdada6ec4dbc2f19ed702bcbd8916a26f8964a2c25790dd65668cfb939d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155701113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7ee85a49e46466a088fa050f4373b9accb131b1b137c3650e9919ecd67d036`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:52ee321733098fccaaf6a0618e45b7dc52f08ce058fb8349984592e05de6bf38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138308211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9bc639ef7ce7d698d0dce478a9a4828085c53c24246570ed03bd3b8871dc0b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:563cc611256b5618ed965af84b42b95da28ea8de2c7105ee1f418161dc1313b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:916ccdc4fb015c163586431e403398e9bbfc9f2826111e325cd004ada298fcb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349058814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c142f83d4bb74d1974a95aed03499ef4f432ebe1986c774237a7dd27127d3483`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:24:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:25:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:25:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:25:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:25:56 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 10:25:56 GMT
ENV ROS2_DISTRO=foxy
# Wed, 05 Oct 2022 10:27:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:27:18 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bed5d7de950633b22457faefa5a82b47b766d96c02665e4faf86d9b7ebe9703`  
		Last Modified: Wed, 05 Oct 2022 10:55:53 GMT  
		Size: 73.3 MB (73322093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e37e53cfffae15445cfdce1b4b7ef7cea4b3e153ea7abf8cd18ebf02b77e34`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 267.4 KB (267375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b37769ea581ebd1d2e907d8c68c8a2c4f7920ce4e81e0099e4165a54aca77`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 2.4 KB (2419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216bc94919c7136aa052456840629454991399309eea61f5b2f7b34471de467c`  
		Last Modified: Wed, 05 Oct 2022 10:55:45 GMT  
		Size: 21.7 MB (21663849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428d94baadca69524a33d3ca807ea019bbad1438b2b7217b4e86ba0e93367003`  
		Last Modified: Wed, 05 Oct 2022 10:56:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccc523540c72f37ce74bb0e501bd649759b2c7dfcb655447fac8913c1517dee`  
		Last Modified: Wed, 05 Oct 2022 10:56:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30e1cb5bcf08c41cd9a4d2e6fe7eaf091057e629ff6f04e3d14c40db29b0048`  
		Last Modified: Wed, 05 Oct 2022 10:56:20 GMT  
		Size: 76.4 MB (76429483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb854b70cf802670e97b4d6ccb7d054bba536f3eb14a57315543c577468c56e`  
		Last Modified: Wed, 05 Oct 2022 10:56:10 GMT  
		Size: 21.7 MB (21671851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dda7b30665fed39bcf488e91c73c1165eea1cd815014048c13330d18959877`  
		Last Modified: Wed, 05 Oct 2022 10:56:06 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9ff7fc96b5af30a5599b70993ddb7041334f53323b4ca7640b57ff9e1e68c4a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.8 MB (316765174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbacdad4c164be3b4c8a143c155c989069e4828ffb5b6bde2b18b7349c7c079b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:50:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:50:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:50:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:50:57 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 13:50:59 GMT
ENV ROS2_DISTRO=foxy
# Wed, 05 Oct 2022 13:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:51:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:51:45 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b933fcbe46312ae813f092369a156c253b1e52cb3a43298b9a4fdbee1eb6fa6b`  
		Last Modified: Wed, 05 Oct 2022 14:14:40 GMT  
		Size: 67.4 MB (67449275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d7c2e640d21fee0497f12b54a0f888d39799eb93389888e1da33e797737919`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 267.3 KB (267323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2d4224582edb4e076612a46599ad24ba3ccfc164b2d512b2006c21094a621`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81d9c31822b3bf7270af1ce9bc509a7516e60401dcfc80333756e3f62d45364`  
		Last Modified: Wed, 05 Oct 2022 14:14:33 GMT  
		Size: 20.4 MB (20366915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f2c8f261aabc480326a91bee38a862a180cfdd89bb015b9d655b99993403e`  
		Last Modified: Wed, 05 Oct 2022 14:14:55 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3614d3bded093673281f432c55f0f746dbe555a0849f2c657164b0dd0a2725`  
		Last Modified: Wed, 05 Oct 2022 14:15:10 GMT  
		Size: 76.3 MB (76271820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301707bbed02236a81c065964e76a9676c5058644e3974e8e8970beeb8e4d4f0`  
		Last Modified: Wed, 05 Oct 2022 14:14:58 GMT  
		Size: 14.1 MB (14098760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3769ba38f03d3d37fa954731a02f330fbfd4cf12cbd6179196026f9909fe85cc`  
		Last Modified: Wed, 05 Oct 2022 14:14:55 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:563cc611256b5618ed965af84b42b95da28ea8de2c7105ee1f418161dc1313b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:916ccdc4fb015c163586431e403398e9bbfc9f2826111e325cd004ada298fcb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349058814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c142f83d4bb74d1974a95aed03499ef4f432ebe1986c774237a7dd27127d3483`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 10:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:24:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:24:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:24:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:24:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:25:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:25:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:25:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:25:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:25:56 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 10:25:56 GMT
ENV ROS2_DISTRO=foxy
# Wed, 05 Oct 2022 10:27:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:27:18 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51876d6577a35c5e59f0be2aaf21be35ae0ccc2ae98272ff4fdc2a4710942e`  
		Last Modified: Wed, 05 Oct 2022 10:55:32 GMT  
		Size: 120.4 MB (120413613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f290f8a7da3fe7da67791a679b225fdfbea4a063f69014d0cc798b572a00606`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bed5d7de950633b22457faefa5a82b47b766d96c02665e4faf86d9b7ebe9703`  
		Last Modified: Wed, 05 Oct 2022 10:55:53 GMT  
		Size: 73.3 MB (73322093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e37e53cfffae15445cfdce1b4b7ef7cea4b3e153ea7abf8cd18ebf02b77e34`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 267.4 KB (267375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b37769ea581ebd1d2e907d8c68c8a2c4f7920ce4e81e0099e4165a54aca77`  
		Last Modified: Wed, 05 Oct 2022 10:55:42 GMT  
		Size: 2.4 KB (2419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216bc94919c7136aa052456840629454991399309eea61f5b2f7b34471de467c`  
		Last Modified: Wed, 05 Oct 2022 10:55:45 GMT  
		Size: 21.7 MB (21663849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428d94baadca69524a33d3ca807ea019bbad1438b2b7217b4e86ba0e93367003`  
		Last Modified: Wed, 05 Oct 2022 10:56:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccc523540c72f37ce74bb0e501bd649759b2c7dfcb655447fac8913c1517dee`  
		Last Modified: Wed, 05 Oct 2022 10:56:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30e1cb5bcf08c41cd9a4d2e6fe7eaf091057e629ff6f04e3d14c40db29b0048`  
		Last Modified: Wed, 05 Oct 2022 10:56:20 GMT  
		Size: 76.4 MB (76429483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb854b70cf802670e97b4d6ccb7d054bba536f3eb14a57315543c577468c56e`  
		Last Modified: Wed, 05 Oct 2022 10:56:10 GMT  
		Size: 21.7 MB (21671851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dda7b30665fed39bcf488e91c73c1165eea1cd815014048c13330d18959877`  
		Last Modified: Wed, 05 Oct 2022 10:56:06 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9ff7fc96b5af30a5599b70993ddb7041334f53323b4ca7640b57ff9e1e68c4a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.8 MB (316765174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbacdad4c164be3b4c8a143c155c989069e4828ffb5b6bde2b18b7349c7c079b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:48:55 GMT
ENV ROS_DISTRO=foxy
# Wed, 05 Oct 2022 13:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:49:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:49:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:49:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:50:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:50:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:50:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:50:57 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 13:50:59 GMT
ENV ROS2_DISTRO=foxy
# Wed, 05 Oct 2022 13:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:51:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:51:45 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761c65c3947a6f0c271454a1a4196e78bc089909ef0635e4fb722f0d26058386`  
		Last Modified: Wed, 05 Oct 2022 14:14:18 GMT  
		Size: 104.6 MB (104627758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d57dc14ffab1724d55720e415410361be4700ed6ecc13df5afc8d58b22afd`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b933fcbe46312ae813f092369a156c253b1e52cb3a43298b9a4fdbee1eb6fa6b`  
		Last Modified: Wed, 05 Oct 2022 14:14:40 GMT  
		Size: 67.4 MB (67449275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d7c2e640d21fee0497f12b54a0f888d39799eb93389888e1da33e797737919`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 267.3 KB (267323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2d4224582edb4e076612a46599ad24ba3ccfc164b2d512b2006c21094a621`  
		Last Modified: Wed, 05 Oct 2022 14:14:30 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81d9c31822b3bf7270af1ce9bc509a7516e60401dcfc80333756e3f62d45364`  
		Last Modified: Wed, 05 Oct 2022 14:14:33 GMT  
		Size: 20.4 MB (20366915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f2c8f261aabc480326a91bee38a862a180cfdd89bb015b9d655b99993403e`  
		Last Modified: Wed, 05 Oct 2022 14:14:55 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3614d3bded093673281f432c55f0f746dbe555a0849f2c657164b0dd0a2725`  
		Last Modified: Wed, 05 Oct 2022 14:15:10 GMT  
		Size: 76.3 MB (76271820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301707bbed02236a81c065964e76a9676c5058644e3974e8e8970beeb8e4d4f0`  
		Last Modified: Wed, 05 Oct 2022 14:14:58 GMT  
		Size: 14.1 MB (14098760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3769ba38f03d3d37fa954731a02f330fbfd4cf12cbd6179196026f9909fe85cc`  
		Last Modified: Wed, 05 Oct 2022 14:14:55 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:671ab05ffcef6bec1b17f2d72ceaf8691d1ec540853afc7d4c2ddd3d4a6a76bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:31e95499a197997474216a4cb9ece22ea610e5b8432d33b081f8a56cdf09b51d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234948199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34842cadd0ae6b77ece4f5f2d3460b0be17b6dd7fae9bada523c9f441d84ecb9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:28:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:28:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325e55da12fa5a2fe5cc77f5f4c49fd8c54a8b75b1371f5a3ad006d8da4cd99`  
		Last Modified: Wed, 05 Oct 2022 10:57:07 GMT  
		Size: 73.3 MB (73278776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c9f33f63d472a14808c264f99830797a829ade91081d5538b5f038d545818`  
		Last Modified: Wed, 05 Oct 2022 10:56:57 GMT  
		Size: 277.8 KB (277810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0f0a76d4c60c66ee530a65c3a89f82c1474b1d942484e6254626fb32b7a38c`  
		Last Modified: Wed, 05 Oct 2022 10:56:56 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9160af9b9ec898e502540ef556ed949674959b38ee20cf5532793f4150c91`  
		Last Modified: Wed, 05 Oct 2022 10:57:00 GMT  
		Size: 22.1 MB (22137635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9823d71d84a6facb9ad6ab94361c78eaafb082eedee10eb50d0fcf03e3196e40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223197069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a96e112da177db105e7ab8a4629e2f05d7ebf4a0f23fba4094e15b8f76174cb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:53:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956f99c4721f7dc25bfe3b1c9c90ce2a2d8b0474b19e342030574fa077dbc98`  
		Last Modified: Wed, 05 Oct 2022 14:15:59 GMT  
		Size: 67.4 MB (67402819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1231122a3faa9e29e7dcfbc07429b9a375bde70cf77017ed38de61d4a42bb924`  
		Last Modified: Wed, 05 Oct 2022 14:15:50 GMT  
		Size: 277.8 KB (277756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5317376816f40e243dc89e1427d6106c53bd777b2ad592afdce65fa1301cdce8`  
		Last Modified: Wed, 05 Oct 2022 14:15:49 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a90f00672da01678118f187b2830f6621555d9e05eddf1d8c10a2d25f967f2`  
		Last Modified: Wed, 05 Oct 2022 14:15:53 GMT  
		Size: 21.5 MB (21458239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:671ab05ffcef6bec1b17f2d72ceaf8691d1ec540853afc7d4c2ddd3d4a6a76bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:31e95499a197997474216a4cb9ece22ea610e5b8432d33b081f8a56cdf09b51d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234948199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34842cadd0ae6b77ece4f5f2d3460b0be17b6dd7fae9bada523c9f441d84ecb9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:28:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:28:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325e55da12fa5a2fe5cc77f5f4c49fd8c54a8b75b1371f5a3ad006d8da4cd99`  
		Last Modified: Wed, 05 Oct 2022 10:57:07 GMT  
		Size: 73.3 MB (73278776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c9f33f63d472a14808c264f99830797a829ade91081d5538b5f038d545818`  
		Last Modified: Wed, 05 Oct 2022 10:56:57 GMT  
		Size: 277.8 KB (277810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0f0a76d4c60c66ee530a65c3a89f82c1474b1d942484e6254626fb32b7a38c`  
		Last Modified: Wed, 05 Oct 2022 10:56:56 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9160af9b9ec898e502540ef556ed949674959b38ee20cf5532793f4150c91`  
		Last Modified: Wed, 05 Oct 2022 10:57:00 GMT  
		Size: 22.1 MB (22137635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9823d71d84a6facb9ad6ab94361c78eaafb082eedee10eb50d0fcf03e3196e40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223197069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a96e112da177db105e7ab8a4629e2f05d7ebf4a0f23fba4094e15b8f76174cb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:53:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956f99c4721f7dc25bfe3b1c9c90ce2a2d8b0474b19e342030574fa077dbc98`  
		Last Modified: Wed, 05 Oct 2022 14:15:59 GMT  
		Size: 67.4 MB (67402819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1231122a3faa9e29e7dcfbc07429b9a375bde70cf77017ed38de61d4a42bb924`  
		Last Modified: Wed, 05 Oct 2022 14:15:50 GMT  
		Size: 277.8 KB (277756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5317376816f40e243dc89e1427d6106c53bd777b2ad592afdce65fa1301cdce8`  
		Last Modified: Wed, 05 Oct 2022 14:15:49 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a90f00672da01678118f187b2830f6621555d9e05eddf1d8c10a2d25f967f2`  
		Last Modified: Wed, 05 Oct 2022 14:15:53 GMT  
		Size: 21.5 MB (21458239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:671ab05ffcef6bec1b17f2d72ceaf8691d1ec540853afc7d4c2ddd3d4a6a76bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:31e95499a197997474216a4cb9ece22ea610e5b8432d33b081f8a56cdf09b51d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234948199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34842cadd0ae6b77ece4f5f2d3460b0be17b6dd7fae9bada523c9f441d84ecb9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:28:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:28:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325e55da12fa5a2fe5cc77f5f4c49fd8c54a8b75b1371f5a3ad006d8da4cd99`  
		Last Modified: Wed, 05 Oct 2022 10:57:07 GMT  
		Size: 73.3 MB (73278776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c9f33f63d472a14808c264f99830797a829ade91081d5538b5f038d545818`  
		Last Modified: Wed, 05 Oct 2022 10:56:57 GMT  
		Size: 277.8 KB (277810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0f0a76d4c60c66ee530a65c3a89f82c1474b1d942484e6254626fb32b7a38c`  
		Last Modified: Wed, 05 Oct 2022 10:56:56 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9160af9b9ec898e502540ef556ed949674959b38ee20cf5532793f4150c91`  
		Last Modified: Wed, 05 Oct 2022 10:57:00 GMT  
		Size: 22.1 MB (22137635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9823d71d84a6facb9ad6ab94361c78eaafb082eedee10eb50d0fcf03e3196e40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223197069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a96e112da177db105e7ab8a4629e2f05d7ebf4a0f23fba4094e15b8f76174cb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:53:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956f99c4721f7dc25bfe3b1c9c90ce2a2d8b0474b19e342030574fa077dbc98`  
		Last Modified: Wed, 05 Oct 2022 14:15:59 GMT  
		Size: 67.4 MB (67402819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1231122a3faa9e29e7dcfbc07429b9a375bde70cf77017ed38de61d4a42bb924`  
		Last Modified: Wed, 05 Oct 2022 14:15:50 GMT  
		Size: 277.8 KB (277756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5317376816f40e243dc89e1427d6106c53bd777b2ad592afdce65fa1301cdce8`  
		Last Modified: Wed, 05 Oct 2022 14:15:49 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a90f00672da01678118f187b2830f6621555d9e05eddf1d8c10a2d25f967f2`  
		Last Modified: Wed, 05 Oct 2022 14:15:53 GMT  
		Size: 21.5 MB (21458239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:0a4d2cfdcc7511b7bb103b5bc38b074b71706792a1cd0bcd6b785c3c9ca74f82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:cb7ef7463a91d118664b763f40f3e4a3aa7ac6114bef24bc0925dd156278f4a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139251521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520cc0d48132237a11f119c67538c538469086a42cf7f674ac73bfc59e9883ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c377541227217e0215aa8042eb861480f28bf127e4a1df6ac7e1bd1033ac4813
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134055898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f30bc0a078ad834182a2ab27c40a5ae2c4edeeb57645071c9b3163fcd3ffcad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:0a4d2cfdcc7511b7bb103b5bc38b074b71706792a1cd0bcd6b785c3c9ca74f82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:cb7ef7463a91d118664b763f40f3e4a3aa7ac6114bef24bc0925dd156278f4a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139251521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520cc0d48132237a11f119c67538c538469086a42cf7f674ac73bfc59e9883ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c377541227217e0215aa8042eb861480f28bf127e4a1df6ac7e1bd1033ac4813
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134055898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f30bc0a078ad834182a2ab27c40a5ae2c4edeeb57645071c9b3163fcd3ffcad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:05c067c0841a86c74153fcfa8dd1a22d5ec41c9b145c9072a369b32c40e78734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:2c20a2ee0c4f6068f57346b1f3acedac2105cd27091b8a440f81ee343a36cf10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330116114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00196654d7606935a1983bf004e12ea7ac742d6fff86f3834602d77053611ee5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:28:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:28:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:29:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:29:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:29:11 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 10:29:11 GMT
ENV ROS2_DISTRO=galactic
# Wed, 05 Oct 2022 10:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:29:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:29:48 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325e55da12fa5a2fe5cc77f5f4c49fd8c54a8b75b1371f5a3ad006d8da4cd99`  
		Last Modified: Wed, 05 Oct 2022 10:57:07 GMT  
		Size: 73.3 MB (73278776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c9f33f63d472a14808c264f99830797a829ade91081d5538b5f038d545818`  
		Last Modified: Wed, 05 Oct 2022 10:56:57 GMT  
		Size: 277.8 KB (277810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0f0a76d4c60c66ee530a65c3a89f82c1474b1d942484e6254626fb32b7a38c`  
		Last Modified: Wed, 05 Oct 2022 10:56:56 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9160af9b9ec898e502540ef556ed949674959b38ee20cf5532793f4150c91`  
		Last Modified: Wed, 05 Oct 2022 10:57:00 GMT  
		Size: 22.1 MB (22137635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07235d4a76cda1362b0738eb1e334ac3bde7bed88bff2930929e7d81234457b`  
		Last Modified: Wed, 05 Oct 2022 10:57:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1919ee6cb43a106ad6556adb87d24ada56ec57246c519d7325e22b1bda93a0`  
		Last Modified: Wed, 05 Oct 2022 10:57:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cfc649897e39fd6d01f08cfa13bca56d18684e9257f1aa8dd8cadb5de5215b`  
		Last Modified: Wed, 05 Oct 2022 10:57:35 GMT  
		Size: 78.7 MB (78702412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4104462282ac7278b053c6afff1967e119382ef6d43ebdb3bad1834de7a981`  
		Last Modified: Wed, 05 Oct 2022 10:57:23 GMT  
		Size: 16.5 MB (16464875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc41efe19dcc3c42cf5550309d17a2313281fb19e49ac6a9700ef83774591ade`  
		Last Modified: Wed, 05 Oct 2022 10:57:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c910804e3fa1439223ed0c67c552d14e326bf7064a773000904f3d23937780f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317407737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9581a373856b8b4cefc18a6aec6600f5c8b14c2cd30fd17381407f2ca8abc33d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:53:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:54:00 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 13:54:01 GMT
ENV ROS2_DISTRO=galactic
# Wed, 05 Oct 2022 13:54:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:54:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:54:51 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956f99c4721f7dc25bfe3b1c9c90ce2a2d8b0474b19e342030574fa077dbc98`  
		Last Modified: Wed, 05 Oct 2022 14:15:59 GMT  
		Size: 67.4 MB (67402819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1231122a3faa9e29e7dcfbc07429b9a375bde70cf77017ed38de61d4a42bb924`  
		Last Modified: Wed, 05 Oct 2022 14:15:50 GMT  
		Size: 277.8 KB (277756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5317376816f40e243dc89e1427d6106c53bd777b2ad592afdce65fa1301cdce8`  
		Last Modified: Wed, 05 Oct 2022 14:15:49 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a90f00672da01678118f187b2830f6621555d9e05eddf1d8c10a2d25f967f2`  
		Last Modified: Wed, 05 Oct 2022 14:15:53 GMT  
		Size: 21.5 MB (21458239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05a5b57afce52501fd8743090826b3937ddca932b9a0b537f904c6a011e3551`  
		Last Modified: Wed, 05 Oct 2022 14:16:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54d7f1aa391ea856e1c1c056ed50ed4b9c2b2a888681732c8725415951e7e60`  
		Last Modified: Wed, 05 Oct 2022 14:16:31 GMT  
		Size: 78.4 MB (78448964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63592baf13af078baa1c931c7c508477a0dfd19142bbef22f18895c1ba8f3356`  
		Last Modified: Wed, 05 Oct 2022 14:16:19 GMT  
		Size: 15.8 MB (15761230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae922e3de5fb8dba104acafb21c858ab1e52a35c4ee38a588d60bcca69ee9b2`  
		Last Modified: Wed, 05 Oct 2022 14:16:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:05c067c0841a86c74153fcfa8dd1a22d5ec41c9b145c9072a369b32c40e78734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:2c20a2ee0c4f6068f57346b1f3acedac2105cd27091b8a440f81ee343a36cf10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330116114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00196654d7606935a1983bf004e12ea7ac742d6fff86f3834602d77053611ee5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:22:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:22:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:22:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:27:33 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 10:28:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:28:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:28:18 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:28:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:28:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:28:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:29:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:29:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:29:11 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 10:29:11 GMT
ENV ROS2_DISTRO=galactic
# Wed, 05 Oct 2022 10:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:29:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:29:48 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62dae53f0e9e7911f61e2af662dfc6c10a32cd5717c41369e1316e320c64345`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01c1f05f8d44c933ce4daf7979f608925683f5ab3dd0b86b37b69af0df974d2`  
		Last Modified: Wed, 05 Oct 2022 10:55:12 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f09aca0821084fd31221ce78f055e457cb666af60a41c8c19af97408974840`  
		Last Modified: Wed, 05 Oct 2022 10:56:47 GMT  
		Size: 104.0 MB (103964019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962252ee5d05117da8058bde3a9410684e471a0d7e8bbe43d008a1be9c3a8590`  
		Last Modified: Wed, 05 Oct 2022 10:56:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325e55da12fa5a2fe5cc77f5f4c49fd8c54a8b75b1371f5a3ad006d8da4cd99`  
		Last Modified: Wed, 05 Oct 2022 10:57:07 GMT  
		Size: 73.3 MB (73278776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c9f33f63d472a14808c264f99830797a829ade91081d5538b5f038d545818`  
		Last Modified: Wed, 05 Oct 2022 10:56:57 GMT  
		Size: 277.8 KB (277810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0f0a76d4c60c66ee530a65c3a89f82c1474b1d942484e6254626fb32b7a38c`  
		Last Modified: Wed, 05 Oct 2022 10:56:56 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9160af9b9ec898e502540ef556ed949674959b38ee20cf5532793f4150c91`  
		Last Modified: Wed, 05 Oct 2022 10:57:00 GMT  
		Size: 22.1 MB (22137635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07235d4a76cda1362b0738eb1e334ac3bde7bed88bff2930929e7d81234457b`  
		Last Modified: Wed, 05 Oct 2022 10:57:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1919ee6cb43a106ad6556adb87d24ada56ec57246c519d7325e22b1bda93a0`  
		Last Modified: Wed, 05 Oct 2022 10:57:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cfc649897e39fd6d01f08cfa13bca56d18684e9257f1aa8dd8cadb5de5215b`  
		Last Modified: Wed, 05 Oct 2022 10:57:35 GMT  
		Size: 78.7 MB (78702412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4104462282ac7278b053c6afff1967e119382ef6d43ebdb3bad1834de7a981`  
		Last Modified: Wed, 05 Oct 2022 10:57:23 GMT  
		Size: 16.5 MB (16464875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc41efe19dcc3c42cf5550309d17a2313281fb19e49ac6a9700ef83774591ade`  
		Last Modified: Wed, 05 Oct 2022 10:57:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c910804e3fa1439223ed0c67c552d14e326bf7064a773000904f3d23937780f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317407737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9581a373856b8b4cefc18a6aec6600f5c8b14c2cd30fd17381407f2ca8abc33d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:48:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:48:53 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:48:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:51:53 GMT
ENV ROS_DISTRO=galactic
# Wed, 05 Oct 2022 13:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:52:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:52:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:52:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:53:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:53:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:53:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:54:00 GMT
ENV ROS1_DISTRO=noetic
# Wed, 05 Oct 2022 13:54:01 GMT
ENV ROS2_DISTRO=galactic
# Wed, 05 Oct 2022 13:54:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:54:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:54:51 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe2304592d4de6867917f39d4e63cc411cb662d76bc30f54ac6c390d02e993`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a824a2931c1c7d4e723b854a254a721dbaaa0d525baef8fc9bffdaa2beacd42`  
		Last Modified: Wed, 05 Oct 2022 14:14:01 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d16a1f7ff237a77f29323231038803c348a1a9f11afc6bb177737dfdcad1c`  
		Last Modified: Wed, 05 Oct 2022 14:15:38 GMT  
		Size: 100.4 MB (100375443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b03d420b9714c9f3dc15cd95ef79baf5b4457aa24c478be8fc2000236b33fc`  
		Last Modified: Wed, 05 Oct 2022 14:15:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956f99c4721f7dc25bfe3b1c9c90ce2a2d8b0474b19e342030574fa077dbc98`  
		Last Modified: Wed, 05 Oct 2022 14:15:59 GMT  
		Size: 67.4 MB (67402819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1231122a3faa9e29e7dcfbc07429b9a375bde70cf77017ed38de61d4a42bb924`  
		Last Modified: Wed, 05 Oct 2022 14:15:50 GMT  
		Size: 277.8 KB (277756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5317376816f40e243dc89e1427d6106c53bd777b2ad592afdce65fa1301cdce8`  
		Last Modified: Wed, 05 Oct 2022 14:15:49 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a90f00672da01678118f187b2830f6621555d9e05eddf1d8c10a2d25f967f2`  
		Last Modified: Wed, 05 Oct 2022 14:15:53 GMT  
		Size: 21.5 MB (21458239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05a5b57afce52501fd8743090826b3937ddca932b9a0b537f904c6a011e3551`  
		Last Modified: Wed, 05 Oct 2022 14:16:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54d7f1aa391ea856e1c1c056ed50ed4b9c2b2a888681732c8725415951e7e60`  
		Last Modified: Wed, 05 Oct 2022 14:16:31 GMT  
		Size: 78.4 MB (78448964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63592baf13af078baa1c931c7c508477a0dfd19142bbef22f18895c1ba8f3356`  
		Last Modified: Wed, 05 Oct 2022 14:16:19 GMT  
		Size: 15.8 MB (15761230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae922e3de5fb8dba104acafb21c858ab1e52a35c4ee38a588d60bcca69ee9b2`  
		Last Modified: Wed, 05 Oct 2022 14:16:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:e7bf15870b85c499ffebbb0e5e7fc733b9d6ac8ebd506cf90a8feb24e455a1a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:fdf2d8cc92e72e6052aa63633e09ce09bcc03e9ef0a65d5e9df7f16590e43a56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262801720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caff7409322c718dbd0b7a41890bf399cc025ce752ce5f0d3c200cec6a66d8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:33:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:33:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:33:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029b0929144e1fbf7711875151abd541f900c4585b654005cb2f30f7c7868386`  
		Last Modified: Wed, 05 Oct 2022 10:58:27 GMT  
		Size: 97.9 MB (97851596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dd89c6f6c80b4bc94a816c40e961d447dd97ed548e5bcdd9acbc88324dbda`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 293.4 KB (293380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d56e31efd937f3db1aa9ed649784bf002d8082e7b4521dea01a898299485e44`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c96f9d9f9a99d848a73ea8e509d25fd737ec31111b3fb98d55502de9f0dd5`  
		Last Modified: Wed, 05 Oct 2022 10:58:15 GMT  
		Size: 23.0 MB (23008452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b52db8801d9e46e66e2f1b84031e242bd5f8c85d836c9ee80ae69bcb98b9e4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255055044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97fa8fa54f8dd58526781db889c6bd8e5ee3e784971669964178b5512fcdb32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:57:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:57:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:57:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:57:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce2c8431570b35ece0db3a51d240fe2781ad038af3c8da3b55b03b4fe8de8ac`  
		Last Modified: Wed, 05 Oct 2022 14:17:22 GMT  
		Size: 95.2 MB (95215132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f80f204207eef3b331605f2054caba003953f6e525e487fe268099461c7eef`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 293.3 KB (293326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44490e7bf336a1cd0e4bbdfc0cb509173c0643c5572dea249d5900bd9121742a`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 2.4 KB (2382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d44d5787adf5963e3ae22a342cafe9f33a160f2cc03b123c4d6996867e0535`  
		Last Modified: Wed, 05 Oct 2022 14:17:12 GMT  
		Size: 22.4 MB (22428695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:1aa7374f9b8280cfb09f2fb4926b43936d4e46e4c61f23fa1c4e9c86e0af6ca2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:239a9ecd2406db4e9e78db070af67069ab44bc96a2bc318927ffd117a97a2584
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1086964233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088a5fabb9c2fab7551dbb7b213641faf6385be95ca962c72c20b357a54f0104`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:33:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:33:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:33:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029b0929144e1fbf7711875151abd541f900c4585b654005cb2f30f7c7868386`  
		Last Modified: Wed, 05 Oct 2022 10:58:27 GMT  
		Size: 97.9 MB (97851596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dd89c6f6c80b4bc94a816c40e961d447dd97ed548e5bcdd9acbc88324dbda`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 293.4 KB (293380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d56e31efd937f3db1aa9ed649784bf002d8082e7b4521dea01a898299485e44`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c96f9d9f9a99d848a73ea8e509d25fd737ec31111b3fb98d55502de9f0dd5`  
		Last Modified: Wed, 05 Oct 2022 10:58:15 GMT  
		Size: 23.0 MB (23008452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6298b8dd92e326429c77e255cee1091ab69cae20cb6df82340970dea80dc785b`  
		Last Modified: Wed, 05 Oct 2022 11:00:24 GMT  
		Size: 824.2 MB (824162513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d33b1eda15a566ef8d7f32e8d9def7e1da4c9bf71d80e0d9ce5495a9737f625
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1036772436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d72876cd51856f6c06f3479fae29de0e96685b3944854f72e4e39bc6c90566a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:57:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:57:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:57:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:57:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce2c8431570b35ece0db3a51d240fe2781ad038af3c8da3b55b03b4fe8de8ac`  
		Last Modified: Wed, 05 Oct 2022 14:17:22 GMT  
		Size: 95.2 MB (95215132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f80f204207eef3b331605f2054caba003953f6e525e487fe268099461c7eef`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 293.3 KB (293326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44490e7bf336a1cd0e4bbdfc0cb509173c0643c5572dea249d5900bd9121742a`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 2.4 KB (2382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d44d5787adf5963e3ae22a342cafe9f33a160f2cc03b123c4d6996867e0535`  
		Last Modified: Wed, 05 Oct 2022 14:17:12 GMT  
		Size: 22.4 MB (22428695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3bcbbe799e24821f61a98ab3360ded019455e6da2828098c9b7ed7d6f5a5d9`  
		Last Modified: Wed, 05 Oct 2022 14:19:54 GMT  
		Size: 781.7 MB (781717392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:1aa7374f9b8280cfb09f2fb4926b43936d4e46e4c61f23fa1c4e9c86e0af6ca2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:239a9ecd2406db4e9e78db070af67069ab44bc96a2bc318927ffd117a97a2584
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1086964233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088a5fabb9c2fab7551dbb7b213641faf6385be95ca962c72c20b357a54f0104`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:33:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:33:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:33:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029b0929144e1fbf7711875151abd541f900c4585b654005cb2f30f7c7868386`  
		Last Modified: Wed, 05 Oct 2022 10:58:27 GMT  
		Size: 97.9 MB (97851596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dd89c6f6c80b4bc94a816c40e961d447dd97ed548e5bcdd9acbc88324dbda`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 293.4 KB (293380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d56e31efd937f3db1aa9ed649784bf002d8082e7b4521dea01a898299485e44`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c96f9d9f9a99d848a73ea8e509d25fd737ec31111b3fb98d55502de9f0dd5`  
		Last Modified: Wed, 05 Oct 2022 10:58:15 GMT  
		Size: 23.0 MB (23008452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6298b8dd92e326429c77e255cee1091ab69cae20cb6df82340970dea80dc785b`  
		Last Modified: Wed, 05 Oct 2022 11:00:24 GMT  
		Size: 824.2 MB (824162513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d33b1eda15a566ef8d7f32e8d9def7e1da4c9bf71d80e0d9ce5495a9737f625
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1036772436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d72876cd51856f6c06f3479fae29de0e96685b3944854f72e4e39bc6c90566a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:57:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:57:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:57:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:57:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce2c8431570b35ece0db3a51d240fe2781ad038af3c8da3b55b03b4fe8de8ac`  
		Last Modified: Wed, 05 Oct 2022 14:17:22 GMT  
		Size: 95.2 MB (95215132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f80f204207eef3b331605f2054caba003953f6e525e487fe268099461c7eef`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 293.3 KB (293326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44490e7bf336a1cd0e4bbdfc0cb509173c0643c5572dea249d5900bd9121742a`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 2.4 KB (2382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d44d5787adf5963e3ae22a342cafe9f33a160f2cc03b123c4d6996867e0535`  
		Last Modified: Wed, 05 Oct 2022 14:17:12 GMT  
		Size: 22.4 MB (22428695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3bcbbe799e24821f61a98ab3360ded019455e6da2828098c9b7ed7d6f5a5d9`  
		Last Modified: Wed, 05 Oct 2022 14:19:54 GMT  
		Size: 781.7 MB (781717392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:e7bf15870b85c499ffebbb0e5e7fc733b9d6ac8ebd506cf90a8feb24e455a1a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:fdf2d8cc92e72e6052aa63633e09ce09bcc03e9ef0a65d5e9df7f16590e43a56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262801720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caff7409322c718dbd0b7a41890bf399cc025ce752ce5f0d3c200cec6a66d8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:33:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:33:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:33:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029b0929144e1fbf7711875151abd541f900c4585b654005cb2f30f7c7868386`  
		Last Modified: Wed, 05 Oct 2022 10:58:27 GMT  
		Size: 97.9 MB (97851596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dd89c6f6c80b4bc94a816c40e961d447dd97ed548e5bcdd9acbc88324dbda`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 293.4 KB (293380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d56e31efd937f3db1aa9ed649784bf002d8082e7b4521dea01a898299485e44`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c96f9d9f9a99d848a73ea8e509d25fd737ec31111b3fb98d55502de9f0dd5`  
		Last Modified: Wed, 05 Oct 2022 10:58:15 GMT  
		Size: 23.0 MB (23008452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b52db8801d9e46e66e2f1b84031e242bd5f8c85d836c9ee80ae69bcb98b9e4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255055044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97fa8fa54f8dd58526781db889c6bd8e5ee3e784971669964178b5512fcdb32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:57:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:57:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:57:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:57:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce2c8431570b35ece0db3a51d240fe2781ad038af3c8da3b55b03b4fe8de8ac`  
		Last Modified: Wed, 05 Oct 2022 14:17:22 GMT  
		Size: 95.2 MB (95215132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f80f204207eef3b331605f2054caba003953f6e525e487fe268099461c7eef`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 293.3 KB (293326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44490e7bf336a1cd0e4bbdfc0cb509173c0643c5572dea249d5900bd9121742a`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 2.4 KB (2382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d44d5787adf5963e3ae22a342cafe9f33a160f2cc03b123c4d6996867e0535`  
		Last Modified: Wed, 05 Oct 2022 14:17:12 GMT  
		Size: 22.4 MB (22428695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:e7bf15870b85c499ffebbb0e5e7fc733b9d6ac8ebd506cf90a8feb24e455a1a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:fdf2d8cc92e72e6052aa63633e09ce09bcc03e9ef0a65d5e9df7f16590e43a56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262801720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caff7409322c718dbd0b7a41890bf399cc025ce752ce5f0d3c200cec6a66d8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:33:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:33:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:33:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029b0929144e1fbf7711875151abd541f900c4585b654005cb2f30f7c7868386`  
		Last Modified: Wed, 05 Oct 2022 10:58:27 GMT  
		Size: 97.9 MB (97851596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dd89c6f6c80b4bc94a816c40e961d447dd97ed548e5bcdd9acbc88324dbda`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 293.4 KB (293380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d56e31efd937f3db1aa9ed649784bf002d8082e7b4521dea01a898299485e44`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c96f9d9f9a99d848a73ea8e509d25fd737ec31111b3fb98d55502de9f0dd5`  
		Last Modified: Wed, 05 Oct 2022 10:58:15 GMT  
		Size: 23.0 MB (23008452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b52db8801d9e46e66e2f1b84031e242bd5f8c85d836c9ee80ae69bcb98b9e4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255055044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97fa8fa54f8dd58526781db889c6bd8e5ee3e784971669964178b5512fcdb32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:57:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:57:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:57:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:57:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce2c8431570b35ece0db3a51d240fe2781ad038af3c8da3b55b03b4fe8de8ac`  
		Last Modified: Wed, 05 Oct 2022 14:17:22 GMT  
		Size: 95.2 MB (95215132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f80f204207eef3b331605f2054caba003953f6e525e487fe268099461c7eef`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 293.3 KB (293326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44490e7bf336a1cd0e4bbdfc0cb509173c0643c5572dea249d5900bd9121742a`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 2.4 KB (2382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d44d5787adf5963e3ae22a342cafe9f33a160f2cc03b123c4d6996867e0535`  
		Last Modified: Wed, 05 Oct 2022 14:17:12 GMT  
		Size: 22.4 MB (22428695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:2be437a0bfcea5aead2093c674390db50edaf49e6231658cf120844d602bbf61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:e9f5409fa1fdbc9056a30ad53163eda953b9d7664a211c15ef3e91d557dc71d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141645846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4c400025ad2a36ba99599ffd8a86840f27147a2d50a17ff245bc09a308f74f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:dbcd22cabd0b7d5b685d0124b75499582924f3e619ecf3e12046df696d4b7040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137115509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1fff96ba234d061182e829199f8154b9ed0b8fb9a76718eed113695c1effb94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:2be437a0bfcea5aead2093c674390db50edaf49e6231658cf120844d602bbf61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e9f5409fa1fdbc9056a30ad53163eda953b9d7664a211c15ef3e91d557dc71d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141645846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4c400025ad2a36ba99599ffd8a86840f27147a2d50a17ff245bc09a308f74f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:dbcd22cabd0b7d5b685d0124b75499582924f3e619ecf3e12046df696d4b7040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137115509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1fff96ba234d061182e829199f8154b9ed0b8fb9a76718eed113695c1effb94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:e7bf15870b85c499ffebbb0e5e7fc733b9d6ac8ebd506cf90a8feb24e455a1a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:fdf2d8cc92e72e6052aa63633e09ce09bcc03e9ef0a65d5e9df7f16590e43a56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262801720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caff7409322c718dbd0b7a41890bf399cc025ce752ce5f0d3c200cec6a66d8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 10:32:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:32:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:32:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:32:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:33:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:33:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:33:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ff840521c5abed0b7ee2eb74488a50f38a6639eb95a973054a41d0fa4eb98`  
		Last Modified: Wed, 05 Oct 2022 10:58:02 GMT  
		Size: 106.2 MB (106210386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc82456ade47aabed8266e54a40aa857a47f06099009e7410d9f1a8462436f`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029b0929144e1fbf7711875151abd541f900c4585b654005cb2f30f7c7868386`  
		Last Modified: Wed, 05 Oct 2022 10:58:27 GMT  
		Size: 97.9 MB (97851596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dd89c6f6c80b4bc94a816c40e961d447dd97ed548e5bcdd9acbc88324dbda`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 293.4 KB (293380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d56e31efd937f3db1aa9ed649784bf002d8082e7b4521dea01a898299485e44`  
		Last Modified: Wed, 05 Oct 2022 10:58:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c96f9d9f9a99d848a73ea8e509d25fd737ec31111b3fb98d55502de9f0dd5`  
		Last Modified: Wed, 05 Oct 2022 10:58:15 GMT  
		Size: 23.0 MB (23008452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b52db8801d9e46e66e2f1b84031e242bd5f8c85d836c9ee80ae69bcb98b9e4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255055044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97fa8fa54f8dd58526781db889c6bd8e5ee3e784971669964178b5512fcdb32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:55:19 GMT
ENV ROS_DISTRO=humble
# Wed, 05 Oct 2022 13:56:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:56:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 13:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:56:19 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:57:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:57:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:57:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 13:57:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77135164a4ca214d5baefbf18732e85e199d498ecc59003672487d9c648b74`  
		Last Modified: Wed, 05 Oct 2022 14:16:58 GMT  
		Size: 104.0 MB (103957828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6965bb2d35a3d18ae4266c452f2a47be3cc9d2dba39a969448e52ad4b37a5b3`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce2c8431570b35ece0db3a51d240fe2781ad038af3c8da3b55b03b4fe8de8ac`  
		Last Modified: Wed, 05 Oct 2022 14:17:22 GMT  
		Size: 95.2 MB (95215132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f80f204207eef3b331605f2054caba003953f6e525e487fe268099461c7eef`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 293.3 KB (293326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44490e7bf336a1cd0e4bbdfc0cb509173c0643c5572dea249d5900bd9121742a`  
		Last Modified: Wed, 05 Oct 2022 14:17:09 GMT  
		Size: 2.4 KB (2382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d44d5787adf5963e3ae22a342cafe9f33a160f2cc03b123c4d6996867e0535`  
		Last Modified: Wed, 05 Oct 2022 14:17:12 GMT  
		Size: 22.4 MB (22428695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:a01392ed8cf43fb99fa539137626bfd50c5b44b63448a4d5ea6b391f6b5b7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:8e83dbb13e46ad46ade95f14a41d9cb1f52b0ded3671ec0ca47da2a75405caa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437522644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19100de5b02016f5969462e71fb3370efde59d2bb6f50e78a774079ca02d19d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a45ac6c100b50466ddc1d7e743fa1245f7fd98846f6029690aea97d10f221e45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (385994420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39885270420308b747b47cac016d290e8ce997f48e27902594c0fb48214d0fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4868ca46db01ab9b479444064b3f4b3919442f2de6fb4f78794359e36ffeb1a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411711887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d006ec586d2e78a0b3c081f1811cfe9cf6ebc2d6e2cec7e0cbbec0e1012473a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:3ec16765c9d5de42dc45a1b452ed02a4a995f9ce5302acdf399943a1ea2ba51c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:1946cf6c8251b3ede407135ff65240b9899a0c8a95c505f0628737e7881f1b45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742878407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ee4b52bee6f5d281b587d8cb4323b6241566389773735252e526a59f5eccf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e954205862ae5cdb5b9218bdf9a5d77ae45554e4d2c990ea5c3fd19cf8554b`  
		Last Modified: Wed, 05 Oct 2022 10:49:50 GMT  
		Size: 305.4 MB (305355763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:d4a2aed0652e148c3323aaf63d7bdbec3ab1a6cd6d46d0b5c259509134524bd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (646023839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf1034097743a12d2ccc90d1828450af36facdf6c4a85c762d45f098854d328`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:51:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b175cc34aa53aebf1e1d4adce550c8bce2cfb95ce33879a16e5f7646f701ba`  
		Last Modified: Thu, 06 Oct 2022 07:00:25 GMT  
		Size: 260.0 MB (260029419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eaa3e6c56b18db14d30b5265127199964e86711e794ce6a97aff1f673eeecd80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.1 MB (703134850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b16a4e6250b3ceb7ce4597efc02b57f3294d8c0f4a5fea3810b2703f925606b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2ce573d6bfab6526367347a90aac300a82c56c3b392c9271d4d28c9a4303c`  
		Last Modified: Wed, 05 Oct 2022 14:08:48 GMT  
		Size: 291.4 MB (291422963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:3ec16765c9d5de42dc45a1b452ed02a4a995f9ce5302acdf399943a1ea2ba51c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:1946cf6c8251b3ede407135ff65240b9899a0c8a95c505f0628737e7881f1b45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742878407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ee4b52bee6f5d281b587d8cb4323b6241566389773735252e526a59f5eccf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e954205862ae5cdb5b9218bdf9a5d77ae45554e4d2c990ea5c3fd19cf8554b`  
		Last Modified: Wed, 05 Oct 2022 10:49:50 GMT  
		Size: 305.4 MB (305355763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:d4a2aed0652e148c3323aaf63d7bdbec3ab1a6cd6d46d0b5c259509134524bd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (646023839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf1034097743a12d2ccc90d1828450af36facdf6c4a85c762d45f098854d328`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:51:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b175cc34aa53aebf1e1d4adce550c8bce2cfb95ce33879a16e5f7646f701ba`  
		Last Modified: Thu, 06 Oct 2022 07:00:25 GMT  
		Size: 260.0 MB (260029419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eaa3e6c56b18db14d30b5265127199964e86711e794ce6a97aff1f673eeecd80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.1 MB (703134850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b16a4e6250b3ceb7ce4597efc02b57f3294d8c0f4a5fea3810b2703f925606b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2ce573d6bfab6526367347a90aac300a82c56c3b392c9271d4d28c9a4303c`  
		Last Modified: Wed, 05 Oct 2022 14:08:48 GMT  
		Size: 291.4 MB (291422963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:b055d0714cec23620b3659f448fedb8f2b541ace510058b681fc7ec916f0e313
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:35d1cf663f1a54a281580c2635a49b9c6d6a88c05d0d274a388119967f5cf002
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448608427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c691edf515ea30216d1741a1934d63e937bf0f449327f950b79fb9b8a7b74a15`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:56:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d82b23298ae87a9d9bc3caf9b4a446fb35de0b2b379eab7db9d03b17e29c17`  
		Last Modified: Wed, 05 Oct 2022 10:48:42 GMT  
		Size: 11.1 MB (11085783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:f41d68e783b7d250adc47fdf91c2d70b5bf9549309e96c6a3aeff32e79def5ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396117676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032becfc9cbe10179ba32714f7356484cde7fb78dd08f85f8380cc46ca85a675`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:49:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335010a557901b56ebbeceac85af817dc563c72e83fe5f3c9d82d92e761187fe`  
		Last Modified: Thu, 06 Oct 2022 06:59:30 GMT  
		Size: 10.1 MB (10123256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6af49c17eb45365833a3015658f71db8cb1496edd7c4196ca5d44baf8cc6bae9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422447622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21b2b650b73f497fe2b2d6860d64416bf68f4185a20ce627275830641d309d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:34:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b70eebce05e703acd0e9cd6a52e2061058ce5b16d05bde10bafa746e1109bd5`  
		Last Modified: Wed, 05 Oct 2022 14:07:54 GMT  
		Size: 10.7 MB (10735735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:b055d0714cec23620b3659f448fedb8f2b541ace510058b681fc7ec916f0e313
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:35d1cf663f1a54a281580c2635a49b9c6d6a88c05d0d274a388119967f5cf002
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448608427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c691edf515ea30216d1741a1934d63e937bf0f449327f950b79fb9b8a7b74a15`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:56:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d82b23298ae87a9d9bc3caf9b4a446fb35de0b2b379eab7db9d03b17e29c17`  
		Last Modified: Wed, 05 Oct 2022 10:48:42 GMT  
		Size: 11.1 MB (11085783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f41d68e783b7d250adc47fdf91c2d70b5bf9549309e96c6a3aeff32e79def5ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396117676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032becfc9cbe10179ba32714f7356484cde7fb78dd08f85f8380cc46ca85a675`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:49:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335010a557901b56ebbeceac85af817dc563c72e83fe5f3c9d82d92e761187fe`  
		Last Modified: Thu, 06 Oct 2022 06:59:30 GMT  
		Size: 10.1 MB (10123256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6af49c17eb45365833a3015658f71db8cb1496edd7c4196ca5d44baf8cc6bae9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422447622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21b2b650b73f497fe2b2d6860d64416bf68f4185a20ce627275830641d309d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:34:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b70eebce05e703acd0e9cd6a52e2061058ce5b16d05bde10bafa746e1109bd5`  
		Last Modified: Wed, 05 Oct 2022 14:07:54 GMT  
		Size: 10.7 MB (10735735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:a01392ed8cf43fb99fa539137626bfd50c5b44b63448a4d5ea6b391f6b5b7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8e83dbb13e46ad46ade95f14a41d9cb1f52b0ded3671ec0ca47da2a75405caa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437522644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19100de5b02016f5969462e71fb3370efde59d2bb6f50e78a774079ca02d19d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:a45ac6c100b50466ddc1d7e743fa1245f7fd98846f6029690aea97d10f221e45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (385994420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39885270420308b747b47cac016d290e8ce997f48e27902594c0fb48214d0fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4868ca46db01ab9b479444064b3f4b3919442f2de6fb4f78794359e36ffeb1a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411711887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d006ec586d2e78a0b3c081f1811cfe9cf6ebc2d6e2cec7e0cbbec0e1012473a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:a01392ed8cf43fb99fa539137626bfd50c5b44b63448a4d5ea6b391f6b5b7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:8e83dbb13e46ad46ade95f14a41d9cb1f52b0ded3671ec0ca47da2a75405caa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437522644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19100de5b02016f5969462e71fb3370efde59d2bb6f50e78a774079ca02d19d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:54:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 09:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291c878123af7c6629193bffe3aef7b2e41bc7e5b6d8d6c195e41a0afa072a2e`  
		Last Modified: Wed, 05 Oct 2022 10:48:23 GMT  
		Size: 70.3 MB (70259758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ad80e5d2bd29146fac7ab104b0a8959214abd2c1e6381db3da5f889ec798c`  
		Last Modified: Wed, 05 Oct 2022 10:48:12 GMT  
		Size: 287.6 KB (287643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13911ccd58f2742aeb456bf670156ec35a6d1bb3670c9ba7d5a709b0201e2388`  
		Last Modified: Wed, 05 Oct 2022 10:48:28 GMT  
		Size: 75.0 MB (74998281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a45ac6c100b50466ddc1d7e743fa1245f7fd98846f6029690aea97d10f221e45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (385994420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39885270420308b747b47cac016d290e8ce997f48e27902594c0fb48214d0fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:48:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c925a21a964fb8486223de78f9a2d457f125c75f70114336548d871ef3aa6e97`  
		Last Modified: Thu, 06 Oct 2022 06:59:08 GMT  
		Size: 54.7 MB (54719854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e6a18e2f88225c6c13f76a00ecd1530583b434fa9c482eee0a2179245adbd`  
		Last Modified: Thu, 06 Oct 2022 06:58:57 GMT  
		Size: 287.8 KB (287786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ace293972247ef40871f854b48d8ab1be13f2c1d04bc8c2d37a6be30a82a5e`  
		Last Modified: Thu, 06 Oct 2022 06:59:13 GMT  
		Size: 64.7 MB (64747626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4868ca46db01ab9b479444064b3f4b3919442f2de6fb4f78794359e36ffeb1a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411711887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d006ec586d2e78a0b3c081f1811cfe9cf6ebc2d6e2cec7e0cbbec0e1012473a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:33:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb232301a9cb5bd90e93d2d742551234aab484877099d191004e68fd52c2939`  
		Last Modified: Wed, 05 Oct 2022 14:07:35 GMT  
		Size: 63.1 MB (63088887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e697dcc64c80657eb9b8cd7f3245242a6c1aa2c256512e00dc7a0b01c50e004`  
		Last Modified: Wed, 05 Oct 2022 14:07:26 GMT  
		Size: 287.6 KB (287598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588145aba131c45bb37457b2bce2eb15ff97b20dc08c8706f0073a5940b0a37`  
		Last Modified: Wed, 05 Oct 2022 14:07:37 GMT  
		Size: 67.0 MB (66998442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:2df63d5d88b85b976800fdb853200e94692c49f344e948ecccc7e4300612be3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:54049e85de367cf82961c3a37fc6af88ae936e8563c1ebfc54203c605c3d414c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291976962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367edf3bdb41bd746cf1277a348f7424c9dc06cbba560ee413e58c4a8375791d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:11cbb2f864a289726b9510d1a9b4e6e7414dfacb9a9d782b9d1e4754293f2056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266239154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d83c28f326a67014793ddf881b3e99269c547c3a86ced293cec9f9fca7d46c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1f76867405b52c64167fb70e1f09efb2123122401686455531be3b1a7ac3221e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281336960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b4b42a718b3881e44324b053aea4b4105bf5b40004428e1ca8c85a6a6ec75e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:2df63d5d88b85b976800fdb853200e94692c49f344e948ecccc7e4300612be3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:54049e85de367cf82961c3a37fc6af88ae936e8563c1ebfc54203c605c3d414c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291976962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367edf3bdb41bd746cf1277a348f7424c9dc06cbba560ee413e58c4a8375791d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:49:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 09:49:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 09:49:44 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 09:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:53:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 09:53:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 09:53:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec163f2e73ca4c7df5142df330fb9169325367e235b65c457afcc3bf320f35`  
		Last Modified: Wed, 05 Oct 2022 10:47:14 GMT  
		Size: 831.0 KB (831002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc154e3f17c6b6f2816c50c8a5bdf831cd4d8813015cacf86568d64746596b6`  
		Last Modified: Wed, 05 Oct 2022 10:47:12 GMT  
		Size: 4.9 MB (4873641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfe6435278fe5856644c183f90cfb982b207bddda62c63a94d6a938acffaa85`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8283d791cae1e7c3329c4a1d8f4bc0476769b04e9ce92d6a97fe84026c059`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60f51f309df710bd88888532e7f25291a9e1d1f54e49a7af43e0771994831f`  
		Last Modified: Wed, 05 Oct 2022 10:48:02 GMT  
		Size: 259.6 MB (259558625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4b730c4ae1b037fe75c6ca063e9c629e1ed238654786a73fabd60b4ed9719`  
		Last Modified: Wed, 05 Oct 2022 10:47:11 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:11cbb2f864a289726b9510d1a9b4e6e7414dfacb9a9d782b9d1e4754293f2056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266239154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d83c28f326a67014793ddf881b3e99269c547c3a86ced293cec9f9fca7d46c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:46:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:46:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:46:42 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Oct 2022 06:48:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:48:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:48:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:48:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f25a09f0aff0cba5b24d07bd5b4c417734fbce77148b7b62042ac54dc95c068`  
		Last Modified: Thu, 06 Oct 2022 06:58:00 GMT  
		Size: 831.1 KB (831144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14397641aa51f3c3aa6ed2c352f3417b3bce0ebaca231e20759c931e3fe38560`  
		Last Modified: Thu, 06 Oct 2022 06:57:58 GMT  
		Size: 4.1 MB (4087217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2d98c80683d1808b546f8ca1a247aecedcea1e9d2460d95343238dfabc896`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670273ddac9f5d6d6c7da9986d18661e88bbbc0126833dcd54f90992f9c9484d`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6664b634c5bf87720b15e47366d33bea9fefdd0032f110f86c336e5ae31a0e`  
		Last Modified: Thu, 06 Oct 2022 06:58:45 GMT  
		Size: 239.0 MB (239013225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074569eb7528b8c52dc9fd001aac258a83c59faaf1830e646c00899e79c3a889`  
		Last Modified: Thu, 06 Oct 2022 06:57:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1f76867405b52c64167fb70e1f09efb2123122401686455531be3b1a7ac3221e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281336960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b4b42a718b3881e44324b053aea4b4105bf5b40004428e1ca8c85a6a6ec75e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:31:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:31:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:31:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:31:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:31:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Oct 2022 13:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:33:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:33:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:33:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe90d911d5615b705080d27fba0823b4f14f420d2d26ab56026456d57781d53`  
		Last Modified: Wed, 05 Oct 2022 14:06:42 GMT  
		Size: 831.4 KB (831396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31110fc43a4ce01227dd0a0453f904b221bd482dc4c0301b8ffa501b18ea30e`  
		Last Modified: Wed, 05 Oct 2022 14:06:40 GMT  
		Size: 4.3 MB (4265721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365507dba87454ad0733144061a0542a771b554c28c0b8ebec0b48db8f8678c`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13820d6a8f15395e7f0229f1db78a33b5cab7627627dcf05a9f5aa25cc4c88a`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3e83df9803da355f686ea14320ce21fd16f2d1d493aa0c23027119f31892e`  
		Last Modified: Wed, 05 Oct 2022 14:07:15 GMT  
		Size: 252.5 MB (252503449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13927152bbda1f9e5e4da3f8f076eeb25177cb22e6347a12dbb859a375a5dfaa`  
		Last Modified: Wed, 05 Oct 2022 14:06:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:fcf95457fdc0e2820875d561fe8abd9159692f5fa32fae3a2211bd0ba3775633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:2bb6821186d86445b5f0b2da7a4ccc36dbc26707ae18b8c8b52184baf0c5fd11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343232868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8ce7cd5edc8f30ba6d15bc589632b6987b60d34f90dc2c31d103b0e700ac8eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:282eece3c6e182e825057bcb769c29ec38c0a3e9b2c9cb0b913ede9dec5a8ccd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289297974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727b6d344ef45add4b6b86083e60223e9bb9840f5052ac125292637db637ef91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:76fd0c9142e5ac05def8adba27f5ae4d8887f4d16e7997c9811a9b93691cadd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322256415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5417df554ee3ec7fde99d2d44aa591593c7532653b7f97faafd2c5d48ec2baf4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:e62310edb60b90b12f8e7bfce08456c83b3c2c2f1b41b5974352365f34ef91fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:fd433ddee6e19535d4222eb87c1c282674e446b33e58ecf9e4e8a16d83a550fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835200384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:494325f2564b03b1d7ebbb1ca7b8bdfddac22ff61863e0eaec0d5650583baee9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:14:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d75818f815178847d6621c476f4f86ec509f7d590cf79978bff7ad8f58d01b`  
		Last Modified: Wed, 05 Oct 2022 10:52:30 GMT  
		Size: 492.0 MB (491967516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3a05ef88d081e15785fcfe16ff2c65f1202d8e5ec15369b110b406ff066c6bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726177866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2302d2ee97aca1cc80e68f815cc9e06f1b146c7567089608a5feb883d948ea4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:57:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed30924832b5259516fe54fa5708a8ae36898b16de1c94f0898baa3d5d3b84a`  
		Last Modified: Thu, 06 Oct 2022 07:03:20 GMT  
		Size: 436.9 MB (436879892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9ad66b6b36c2b6ca4ecc31c4f8f1f19bccceb47cf271dd5441c9dbac84ee8ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.8 MB (784795707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d38a613da5f472621d5e0844eafee839f3f0dd60170e73750a822cba8e910cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:42:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74469c08d264edcc5ee135c5451f9ae9f9636a408d721ae64bb3afcbf69ee13b`  
		Last Modified: Wed, 05 Oct 2022 14:11:25 GMT  
		Size: 462.5 MB (462539292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:8abadae98bba78dd9625bccd1030e8305e7920b8010787a4148efce7fea1c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:08e06ab6cf9e9bc92ce20c5db639653a5ccc4a39f0a644ca0be8ba9a8eae2c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.4 MB (951411608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965503cf726ff4ce7ebfb99527bd04f50700b3d7f5552dd3346d4b8461cc9d0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:15:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:15:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:15:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:16:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:16:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:16:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:17:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:17:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:21:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341aa83c173ccc7896ed46aadb5f8da7ef58882bd50ab70db04adad01c7dd54`  
		Last Modified: Wed, 05 Oct 2022 10:52:43 GMT  
		Size: 10.9 MB (10893675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707ffddc54db884ea0f0b8d3dcb59efecf4b23f05ca9678cdb9093afeb503ed`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189ff615727a275e72ab0b25ee32ab5bbaf9038ec984ac9590b05ec0bd699420`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02002ab3d47e892389b5c1698d3762ba599087c17a75d1c89b38eba2d10e9e73`  
		Last Modified: Wed, 05 Oct 2022 10:53:15 GMT  
		Size: 239.2 MB (239205312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b538c244b3c01ac7f43cbbe81f3828c21d135d04e3f09c2be3cbd996f74e2d`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df699501c681c16e834b1d4c6a0020da7a337123f2599fa0138c7a689abe2c00`  
		Last Modified: Wed, 05 Oct 2022 10:53:34 GMT  
		Size: 86.6 MB (86571557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c877ef0ff6f06ed582cc68bf1bb2a9f3febf8e8d6812c86c77fa110bf09fe22`  
		Last Modified: Wed, 05 Oct 2022 10:53:22 GMT  
		Size: 324.6 KB (324645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6360754d0398a4f26fe2e6909f0d860b818f474a42c16d8f1fb6232def5a53d`  
		Last Modified: Wed, 05 Oct 2022 10:53:33 GMT  
		Size: 76.0 MB (75976232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829343866cdb6d39fe9e6d8009e2e081875e38ce8f48936b829813b8b77dcf1`  
		Last Modified: Wed, 05 Oct 2022 10:55:04 GMT  
		Size: 488.0 MB (487996673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0be734205fcd3bb5d8d7b494b2480ee3c501e8e7bc80a22086c5fae168d0ff18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.7 MB (867691466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0407a6c31b234440c08346172e561c78fdef9da60394cfc61d02ee81616aff43`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:42:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:42:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:42:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:42:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:42:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:42:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:43:35 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:43:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:43:38 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:44:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:44:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:45:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c286841822dd708cc8ec03c64947552384e955fad5e3df9a73a5acab4aaaed`  
		Last Modified: Wed, 05 Oct 2022 14:11:38 GMT  
		Size: 10.7 MB (10689488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b51b46470fae12ab22dbf0e0f68d92e335b5d2aec01faf4694f688dcff7ed7e`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01f93551ac4426be901cafe628cfa60e541d98154404fcba3cb02cde1d85358`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a850fdf218d14508c13532bd2745504750003968ec91b47bbc2a16d38af0791f`  
		Last Modified: Wed, 05 Oct 2022 14:12:09 GMT  
		Size: 184.4 MB (184402359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46befb9f0b1823e66932ff7e6bd3b3f7ef17e0115617e47457b2e68aa6db3103`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70142cef45c79ed6c16def65c939723b912688d777616cd8f0394a0a9bed62b`  
		Last Modified: Wed, 05 Oct 2022 14:12:28 GMT  
		Size: 84.4 MB (84371054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec293e0c6336ccbd0d0986af98ef8fd2f6e8caebfc5454d01a8d50bf39f3310`  
		Last Modified: Wed, 05 Oct 2022 14:12:17 GMT  
		Size: 324.6 KB (324579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdd5b15718815c6b2b180f7ba28bb586c4071861d49a281db790d1263561842`  
		Last Modified: Wed, 05 Oct 2022 14:12:26 GMT  
		Size: 73.9 MB (73865277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce03a7da0d66f047902e88c4c2a4af4a8a6d8ab4e8e457debc9fbdebb20bfc3e`  
		Last Modified: Wed, 05 Oct 2022 14:13:53 GMT  
		Size: 464.8 MB (464807456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:e62310edb60b90b12f8e7bfce08456c83b3c2c2f1b41b5974352365f34ef91fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:fd433ddee6e19535d4222eb87c1c282674e446b33e58ecf9e4e8a16d83a550fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835200384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:494325f2564b03b1d7ebbb1ca7b8bdfddac22ff61863e0eaec0d5650583baee9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:14:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d75818f815178847d6621c476f4f86ec509f7d590cf79978bff7ad8f58d01b`  
		Last Modified: Wed, 05 Oct 2022 10:52:30 GMT  
		Size: 492.0 MB (491967516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3a05ef88d081e15785fcfe16ff2c65f1202d8e5ec15369b110b406ff066c6bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726177866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2302d2ee97aca1cc80e68f815cc9e06f1b146c7567089608a5feb883d948ea4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:57:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed30924832b5259516fe54fa5708a8ae36898b16de1c94f0898baa3d5d3b84a`  
		Last Modified: Thu, 06 Oct 2022 07:03:20 GMT  
		Size: 436.9 MB (436879892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9ad66b6b36c2b6ca4ecc31c4f8f1f19bccceb47cf271dd5441c9dbac84ee8ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.8 MB (784795707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d38a613da5f472621d5e0844eafee839f3f0dd60170e73750a822cba8e910cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:42:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74469c08d264edcc5ee135c5451f9ae9f9636a408d721ae64bb3afcbf69ee13b`  
		Last Modified: Wed, 05 Oct 2022 14:11:25 GMT  
		Size: 462.5 MB (462539292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:4b8e2a7b94510cdef56a88d575a6e45a60bac243169ea909e128aa708bb74e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:b02a93370486adbbb4845c933381378c1fffa0ab564b970622b98bbaa5daa8c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359094351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7bbf5f7cc9477ad5cd3dfbf2bbfaec244cf3ae7e28b5aa13d610d7c3bf5f96a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:08:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a69bb95b74148eb43365cb23e48cffb03e4ff7e3a6191eb50efaa36bcec1332`  
		Last Modified: Wed, 05 Oct 2022 10:51:07 GMT  
		Size: 15.9 MB (15861483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:931a8f67e0e7779bbadc154d28cb081ecc3163db2b77ac9539c413644b6ceff5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303363136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205efb50cd40a2dadaee4531776d2a257c8fce1a9728465df5468491f976aac3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:54:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4213011fc7a49cf580c896c00969f42891823b1dbe5356b6a627e03ac4bd6e13`  
		Last Modified: Thu, 06 Oct 2022 07:01:58 GMT  
		Size: 14.1 MB (14065162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbf89f5bcbf5baf8a786e0945237b78bac1cc8cefb7ac4b9876ec84037d77ded
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337705362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da55244b8dc759186bfe3eb5d355819b03d26aa18833e3c469b3de63690a940e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:39:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635d5818920d712c2d0c966e72310e1423cd89ced677c40f6f31ddadb8bf6b8f`  
		Last Modified: Wed, 05 Oct 2022 14:10:07 GMT  
		Size: 15.4 MB (15448947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:c0a507261c2521305e155f1d4b1b55578ceb3e5a52f29557546c766817d525c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:26ee7d27c07e131afbe2b0d8df3a479c7e41931f5116c36f0815ebe5952b9d6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.9 MB (484863624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0a98162000767aad3a21a3320626245a63247696805bb8e28bb08b39a7c999`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:15:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:15:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:15:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:16:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:16:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:16:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:17:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:17:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:18:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341aa83c173ccc7896ed46aadb5f8da7ef58882bd50ab70db04adad01c7dd54`  
		Last Modified: Wed, 05 Oct 2022 10:52:43 GMT  
		Size: 10.9 MB (10893675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707ffddc54db884ea0f0b8d3dcb59efecf4b23f05ca9678cdb9093afeb503ed`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189ff615727a275e72ab0b25ee32ab5bbaf9038ec984ac9590b05ec0bd699420`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02002ab3d47e892389b5c1698d3762ba599087c17a75d1c89b38eba2d10e9e73`  
		Last Modified: Wed, 05 Oct 2022 10:53:15 GMT  
		Size: 239.2 MB (239205312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b538c244b3c01ac7f43cbbe81f3828c21d135d04e3f09c2be3cbd996f74e2d`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df699501c681c16e834b1d4c6a0020da7a337123f2599fa0138c7a689abe2c00`  
		Last Modified: Wed, 05 Oct 2022 10:53:34 GMT  
		Size: 86.6 MB (86571557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c877ef0ff6f06ed582cc68bf1bb2a9f3febf8e8d6812c86c77fa110bf09fe22`  
		Last Modified: Wed, 05 Oct 2022 10:53:22 GMT  
		Size: 324.6 KB (324645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6360754d0398a4f26fe2e6909f0d860b818f474a42c16d8f1fb6232def5a53d`  
		Last Modified: Wed, 05 Oct 2022 10:53:33 GMT  
		Size: 76.0 MB (75976232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893fae4daed6c6414cc2281b66f2fc63c8c815eff25b0833189f66bfbef8a40`  
		Last Modified: Wed, 05 Oct 2022 10:53:44 GMT  
		Size: 21.4 MB (21448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3b603a162a01cffc2f94f0638445bdb64192217fb369bb1d3cf5b3341a353b75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423991607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c82425e01996b0f75a886f464dbcb66332c2a722fb5c343e861996462a994d70`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:42:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:42:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:42:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:42:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:42:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:42:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:43:35 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:43:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:43:38 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:44:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:44:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:45:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:45:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c286841822dd708cc8ec03c64947552384e955fad5e3df9a73a5acab4aaaed`  
		Last Modified: Wed, 05 Oct 2022 14:11:38 GMT  
		Size: 10.7 MB (10689488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b51b46470fae12ab22dbf0e0f68d92e335b5d2aec01faf4694f688dcff7ed7e`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01f93551ac4426be901cafe628cfa60e541d98154404fcba3cb02cde1d85358`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a850fdf218d14508c13532bd2745504750003968ec91b47bbc2a16d38af0791f`  
		Last Modified: Wed, 05 Oct 2022 14:12:09 GMT  
		Size: 184.4 MB (184402359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46befb9f0b1823e66932ff7e6bd3b3f7ef17e0115617e47457b2e68aa6db3103`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70142cef45c79ed6c16def65c939723b912688d777616cd8f0394a0a9bed62b`  
		Last Modified: Wed, 05 Oct 2022 14:12:28 GMT  
		Size: 84.4 MB (84371054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec293e0c6336ccbd0d0986af98ef8fd2f6e8caebfc5454d01a8d50bf39f3310`  
		Last Modified: Wed, 05 Oct 2022 14:12:17 GMT  
		Size: 324.6 KB (324579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdd5b15718815c6b2b180f7ba28bb586c4071861d49a281db790d1263561842`  
		Last Modified: Wed, 05 Oct 2022 14:12:26 GMT  
		Size: 73.9 MB (73865277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6113ec2fc7cc5403f1bec46f71179910d1b80ae4844ca9e0759bbaa64a354ea5`  
		Last Modified: Wed, 05 Oct 2022 14:12:38 GMT  
		Size: 21.1 MB (21107597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:4b8e2a7b94510cdef56a88d575a6e45a60bac243169ea909e128aa708bb74e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:b02a93370486adbbb4845c933381378c1fffa0ab564b970622b98bbaa5daa8c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359094351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7bbf5f7cc9477ad5cd3dfbf2bbfaec244cf3ae7e28b5aa13d610d7c3bf5f96a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:08:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a69bb95b74148eb43365cb23e48cffb03e4ff7e3a6191eb50efaa36bcec1332`  
		Last Modified: Wed, 05 Oct 2022 10:51:07 GMT  
		Size: 15.9 MB (15861483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:931a8f67e0e7779bbadc154d28cb081ecc3163db2b77ac9539c413644b6ceff5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303363136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205efb50cd40a2dadaee4531776d2a257c8fce1a9728465df5468491f976aac3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:54:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4213011fc7a49cf580c896c00969f42891823b1dbe5356b6a627e03ac4bd6e13`  
		Last Modified: Thu, 06 Oct 2022 07:01:58 GMT  
		Size: 14.1 MB (14065162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbf89f5bcbf5baf8a786e0945237b78bac1cc8cefb7ac4b9876ec84037d77ded
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337705362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da55244b8dc759186bfe3eb5d355819b03d26aa18833e3c469b3de63690a940e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:39:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635d5818920d712c2d0c966e72310e1423cd89ced677c40f6f31ddadb8bf6b8f`  
		Last Modified: Wed, 05 Oct 2022 14:10:07 GMT  
		Size: 15.4 MB (15448947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:fcf95457fdc0e2820875d561fe8abd9159692f5fa32fae3a2211bd0ba3775633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2bb6821186d86445b5f0b2da7a4ccc36dbc26707ae18b8c8b52184baf0c5fd11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343232868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8ce7cd5edc8f30ba6d15bc589632b6987b60d34f90dc2c31d103b0e700ac8eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:282eece3c6e182e825057bcb769c29ec38c0a3e9b2c9cb0b913ede9dec5a8ccd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289297974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727b6d344ef45add4b6b86083e60223e9bb9840f5052ac125292637db637ef91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:76fd0c9142e5ac05def8adba27f5ae4d8887f4d16e7997c9811a9b93691cadd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322256415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5417df554ee3ec7fde99d2d44aa591593c7532653b7f97faafd2c5d48ec2baf4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:e640a1d4b99df8eb28d2077a17417bce953ca1156e72b84d7ed99dffd77009cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:23a065cfb6cc6467d16377f4775b9f465f61d34a7663caf3f7923c0993b949a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463414935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd7771570486dc2f32baa1402d5b76bc4eb21838c9af5a80c83135545b23233e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:15:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:15:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:15:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:16:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:16:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:16:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:17:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:17:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341aa83c173ccc7896ed46aadb5f8da7ef58882bd50ab70db04adad01c7dd54`  
		Last Modified: Wed, 05 Oct 2022 10:52:43 GMT  
		Size: 10.9 MB (10893675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707ffddc54db884ea0f0b8d3dcb59efecf4b23f05ca9678cdb9093afeb503ed`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189ff615727a275e72ab0b25ee32ab5bbaf9038ec984ac9590b05ec0bd699420`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02002ab3d47e892389b5c1698d3762ba599087c17a75d1c89b38eba2d10e9e73`  
		Last Modified: Wed, 05 Oct 2022 10:53:15 GMT  
		Size: 239.2 MB (239205312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b538c244b3c01ac7f43cbbe81f3828c21d135d04e3f09c2be3cbd996f74e2d`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df699501c681c16e834b1d4c6a0020da7a337123f2599fa0138c7a689abe2c00`  
		Last Modified: Wed, 05 Oct 2022 10:53:34 GMT  
		Size: 86.6 MB (86571557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c877ef0ff6f06ed582cc68bf1bb2a9f3febf8e8d6812c86c77fa110bf09fe22`  
		Last Modified: Wed, 05 Oct 2022 10:53:22 GMT  
		Size: 324.6 KB (324645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6360754d0398a4f26fe2e6909f0d860b818f474a42c16d8f1fb6232def5a53d`  
		Last Modified: Wed, 05 Oct 2022 10:53:33 GMT  
		Size: 76.0 MB (75976232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4e6ad0ca4781fdc64d09a1648afd8f8db480941c55c7584bb64df0449bfe27d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.9 MB (402884010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943c47c820a9c53838514e9638c0e4218b301b3a485b2ded7c73b51629dc36e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:42:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:42:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:42:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:42:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:42:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:42:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:43:35 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:43:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:43:38 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:44:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:44:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:45:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c286841822dd708cc8ec03c64947552384e955fad5e3df9a73a5acab4aaaed`  
		Last Modified: Wed, 05 Oct 2022 14:11:38 GMT  
		Size: 10.7 MB (10689488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b51b46470fae12ab22dbf0e0f68d92e335b5d2aec01faf4694f688dcff7ed7e`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01f93551ac4426be901cafe628cfa60e541d98154404fcba3cb02cde1d85358`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a850fdf218d14508c13532bd2745504750003968ec91b47bbc2a16d38af0791f`  
		Last Modified: Wed, 05 Oct 2022 14:12:09 GMT  
		Size: 184.4 MB (184402359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46befb9f0b1823e66932ff7e6bd3b3f7ef17e0115617e47457b2e68aa6db3103`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70142cef45c79ed6c16def65c939723b912688d777616cd8f0394a0a9bed62b`  
		Last Modified: Wed, 05 Oct 2022 14:12:28 GMT  
		Size: 84.4 MB (84371054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec293e0c6336ccbd0d0986af98ef8fd2f6e8caebfc5454d01a8d50bf39f3310`  
		Last Modified: Wed, 05 Oct 2022 14:12:17 GMT  
		Size: 324.6 KB (324579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdd5b15718815c6b2b180f7ba28bb586c4071861d49a281db790d1263561842`  
		Last Modified: Wed, 05 Oct 2022 14:12:26 GMT  
		Size: 73.9 MB (73865277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:fcf95457fdc0e2820875d561fe8abd9159692f5fa32fae3a2211bd0ba3775633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:2bb6821186d86445b5f0b2da7a4ccc36dbc26707ae18b8c8b52184baf0c5fd11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343232868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8ce7cd5edc8f30ba6d15bc589632b6987b60d34f90dc2c31d103b0e700ac8eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:06:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:06:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c711ad2d8e864145c52c8810c7eaacae497a7a0eb81da4ede8668228e1674`  
		Last Modified: Wed, 05 Oct 2022 10:50:48 GMT  
		Size: 50.9 MB (50940474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a6fe92784306c9f1453b6a855ad51a4ec6eed4ac1c90ea59048368531974f`  
		Last Modified: Wed, 05 Oct 2022 10:50:40 GMT  
		Size: 329.9 KB (329911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45a8a3d4e2bf3f49eace9665b5b4fcb4dcf67a51bdfabd6a30c6a1e58420b9`  
		Last Modified: Wed, 05 Oct 2022 10:50:52 GMT  
		Size: 79.6 MB (79603231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:282eece3c6e182e825057bcb769c29ec38c0a3e9b2c9cb0b913ede9dec5a8ccd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289297974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727b6d344ef45add4b6b86083e60223e9bb9840f5052ac125292637db637ef91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:53:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Oct 2022 06:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1461e09b998de0d3b7ae285e2a3bb8bcb1b889f8a12f832e208d7ec8d3bfe847`  
		Last Modified: Thu, 06 Oct 2022 07:01:36 GMT  
		Size: 40.5 MB (40505592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e355cb57c65a1dc870c88f7e383d6a76770d5f6563b605a9a96dc5ceb24b3a`  
		Last Modified: Thu, 06 Oct 2022 07:01:28 GMT  
		Size: 329.9 KB (329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b621043424762e62d798dd71533b7835ccd3741e94dcdc7fbbdd3ca4f723`  
		Last Modified: Thu, 06 Oct 2022 07:01:40 GMT  
		Size: 60.5 MB (60479707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:76fd0c9142e5ac05def8adba27f5ae4d8887f4d16e7997c9811a9b93691cadd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322256415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5417df554ee3ec7fde99d2d44aa591593c7532653b7f97faafd2c5d48ec2baf4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 13:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814635c2ec9fc6aa1c79542be862549465c5ec04cef8ec399952b79e14fe736`  
		Last Modified: Wed, 05 Oct 2022 14:09:46 GMT  
		Size: 45.0 MB (44987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762c4f58b5522b0b2e4a82a4b02573353cdb815242b32b47ea696270c4f74f0`  
		Last Modified: Wed, 05 Oct 2022 14:09:40 GMT  
		Size: 329.8 KB (329844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7389f48d507d2a20ca2a184d421e98d9717ff8bd42ce2a9e76b6b153dfc2ee27`  
		Last Modified: Wed, 05 Oct 2022 14:09:50 GMT  
		Size: 71.8 MB (71753417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:86dbf9b47b74d62f9ed472b94ed961b366432ce81a4aa277c05bf31b60e4c4b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9454832098cb04c4508f2bbe5023c1b806e7eb4c08b6b8ce43e6a63dec01506c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212359252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba7534ada8b86cd4acbdc599729fed2e3c729ae0872bdc78c5129dac1c1054f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:67ea8f522d8e90ade44c0d45a623b182c7dbb9f48f4b567f1079e6d3136ca48c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187982732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7c3f4179402fe66a367adbf02ca6941b11a372f4111ef176ab7c3c7de1f500`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f89895ef429256f804633dc9c6e2ab38c57680aa920bc071d8f71efbc5020e42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.2 MB (205185193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9baaec59cb59cfd4a6e30cff261cc9b7590948f136dad75047c09c4eff7a60ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:3cb2adbe06a290ae95a5eaac10fb9bc6299b2fa0b6f2498d379c23c3e586a64d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:87d2bdaa561457cf0edfa896b1fac43a9c8ad055485d6a141d18a28c4d563533
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300542501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a565f412c169c509918d7910d2b507e182a8b97109ab9cc2e42146fe2152b95a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:15:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:15:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:15:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:15:10 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:16:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:16:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:16:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341aa83c173ccc7896ed46aadb5f8da7ef58882bd50ab70db04adad01c7dd54`  
		Last Modified: Wed, 05 Oct 2022 10:52:43 GMT  
		Size: 10.9 MB (10893675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707ffddc54db884ea0f0b8d3dcb59efecf4b23f05ca9678cdb9093afeb503ed`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189ff615727a275e72ab0b25ee32ab5bbaf9038ec984ac9590b05ec0bd699420`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02002ab3d47e892389b5c1698d3762ba599087c17a75d1c89b38eba2d10e9e73`  
		Last Modified: Wed, 05 Oct 2022 10:53:15 GMT  
		Size: 239.2 MB (239205312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b538c244b3c01ac7f43cbbe81f3828c21d135d04e3f09c2be3cbd996f74e2d`  
		Last Modified: Wed, 05 Oct 2022 10:52:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:afc032e9fa26896123d80250930a58078ebf41c1ff40beba11ea11c54d5a2193
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244323100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746f7bae696247627d344c0afb30c2178be92cef192a0b9831736fa090473713`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:42:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:42:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:42:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:42:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:42:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:42:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:43:35 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:43:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:43:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c286841822dd708cc8ec03c64947552384e955fad5e3df9a73a5acab4aaaed`  
		Last Modified: Wed, 05 Oct 2022 14:11:38 GMT  
		Size: 10.7 MB (10689488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b51b46470fae12ab22dbf0e0f68d92e335b5d2aec01faf4694f688dcff7ed7e`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01f93551ac4426be901cafe628cfa60e541d98154404fcba3cb02cde1d85358`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a850fdf218d14508c13532bd2745504750003968ec91b47bbc2a16d38af0791f`  
		Last Modified: Wed, 05 Oct 2022 14:12:09 GMT  
		Size: 184.4 MB (184402359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46befb9f0b1823e66932ff7e6bd3b3f7ef17e0115617e47457b2e68aa6db3103`  
		Last Modified: Wed, 05 Oct 2022 14:11:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:86dbf9b47b74d62f9ed472b94ed961b366432ce81a4aa277c05bf31b60e4c4b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:9454832098cb04c4508f2bbe5023c1b806e7eb4c08b6b8ce43e6a63dec01506c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212359252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba7534ada8b86cd4acbdc599729fed2e3c729ae0872bdc78c5129dac1c1054f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:02:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:02:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 10:02:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:02:52 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 10:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:05:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 10:05:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:05:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db398de1191a2231a78b6d5d54baa0f980aa763df67adb3394a7269111109671`  
		Last Modified: Wed, 05 Oct 2022 10:50:03 GMT  
		Size: 1.2 MB (1163849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d2c75c8d50e5aa3470df0fc55d0148e41867398126d721472b626f05229661`  
		Last Modified: Wed, 05 Oct 2022 10:50:01 GMT  
		Size: 5.5 MB (5546788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903c62e1337e2dd7c72c1e20fc53356cb226565140bd53279940a0824dfd9fe`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68edbd1d0652c7c600df686df53d5de7acd8204dfdaa0021473d00b987edf1`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d57e521255204934b128030a0d4d356e8969e88e5db0e946889bffaae21ee`  
		Last Modified: Wed, 05 Oct 2022 10:50:30 GMT  
		Size: 177.1 MB (177071749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6428d2dd8bfe4fac9ded18b38507319ecee51621fdf191793d6687512c69d86`  
		Last Modified: Wed, 05 Oct 2022 10:50:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:67ea8f522d8e90ade44c0d45a623b182c7dbb9f48f4b567f1079e6d3136ca48c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187982732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7c3f4179402fe66a367adbf02ca6941b11a372f4111ef176ab7c3c7de1f500`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:52:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 06 Oct 2022 06:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Oct 2022 06:52:16 GMT
ENV ROS_DISTRO=noetic
# Thu, 06 Oct 2022 06:53:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:53:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 06 Oct 2022 06:53:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Oct 2022 06:53:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ab6ac546133bf21e51dc29641d455c42144b184821f494258ff1ec514556c`  
		Last Modified: Thu, 06 Oct 2022 07:00:40 GMT  
		Size: 1.2 MB (1163905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4706759f53c150848596edb49143a211c7e072793acea609cc8e9c0f267c4e3e`  
		Last Modified: Thu, 06 Oct 2022 07:00:38 GMT  
		Size: 4.7 MB (4675577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b0360f8c716b3c493ff9708abd3c165f9de06193430830ea64d829b1a6ac2`  
		Last Modified: Thu, 06 Oct 2022 07:00:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd789251f14b7842f745c35075b3e7f88a5aa3fb3b005a3bd0fde7d8f285d7f`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24248fc7fc767d03259bb795d6c177495b4f61cdb1ddcc6a6bb9bb7dcd5958db`  
		Last Modified: Thu, 06 Oct 2022 07:01:15 GMT  
		Size: 157.6 MB (157550749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1b296e1c261f003a529641cc88d1393116b3a0b1f7853da9463a2e9c16df7c`  
		Last Modified: Thu, 06 Oct 2022 07:00:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f89895ef429256f804633dc9c6e2ab38c57680aa920bc071d8f71efbc5020e42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.2 MB (205185193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9baaec59cb59cfd4a6e30cff261cc9b7590948f136dad75047c09c4eff7a60ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:36:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Oct 2022 13:36:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:36:53 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 13:36:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Oct 2022 13:37:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:37:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 05 Oct 2022 13:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 13:37:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2066945f278504a3fbe15500f54112556cb9e9febb0b4d07edd644ecbae9209c`  
		Last Modified: Wed, 05 Oct 2022 14:09:02 GMT  
		Size: 1.2 MB (1164049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ca1624225b52b4e52d61f82b52ba0653fdefd1bcde8f1017fc0031f256a5d`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 5.3 MB (5322416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0727eb08e94e95fafae4d8d0079ee1413dc8ff544022ff06d844f4a53bf3c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf931507240c54649243355c092bd81e83eae6916ab26a7620f410132c2d47c`  
		Last Modified: Wed, 05 Oct 2022 14:09:00 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991837517e4c0d5001d2caa2a90cf5e70018524cf2ad724b9cf736dc76eb1d05`  
		Last Modified: Wed, 05 Oct 2022 14:09:29 GMT  
		Size: 171.5 MB (171504736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4fe51a6dd429e99d46144fc5ddd118e6c466b37ffb21e3942c6fb1bcb67ac`  
		Last Modified: Wed, 05 Oct 2022 14:08:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:c2ed7361c46259c8fd1b74efd17eff5ec2610e2376f25c6c178cbb0f455f0153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:0840fe8af38c3bd1f0447f886a73d7896d178e41bc5030948863ad8642c559af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263178182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9edb8205b6372daa73ead068a4158fc78e31fbab557c826bcd3dfd2473dcd91d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:43:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:43:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:43:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1a884c0500e4a2eccb5a2a364d8d1cdc8c80689d7292e492c144c4dee8f69`  
		Last Modified: Wed, 05 Oct 2022 11:01:16 GMT  
		Size: 97.9 MB (97851974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420841bcfe85d95f042c1930c98a9f177ba6b518fc1c10bd66c341017785ccf5`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 287.9 KB (287858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896c641876dd5da58d9cd9d3b9c73d0a464a3dcb760e5efa747239c51261735`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b4eca3f72bccb69be61064fc7d85e752e7d5c0d0cf14b71a6fe5dea6feb8c`  
		Last Modified: Wed, 05 Oct 2022 11:01:06 GMT  
		Size: 23.2 MB (23226838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33669f7bf08ec323d17bd2d63532f30fe9982bbb13f7cf849dd97b000c8a1827
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255407846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be0b50bb3221f9dcf4ace9413a489fa328657908bfeada9464bac70440cca785`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:01:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 14:01:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 14:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2767f80cc9b7f92921da87e086a643d8d80b257ce273716d8795816f765216`  
		Last Modified: Wed, 05 Oct 2022 14:20:48 GMT  
		Size: 95.2 MB (95215484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c34644006693e54ff50141efeaec2467a06586f1f28d4e4874485d96ad999`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 287.8 KB (287799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9377d158c53ca57fb20de69f4e1e1f1bb1741c856365104a808553e58c611ecc`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 2.4 KB (2353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f3f8b1a658efb974ec2a2c92261fc0ca9d5ad9d4eecf003b8752e7b82ab271`  
		Last Modified: Wed, 05 Oct 2022 14:20:38 GMT  
		Size: 22.6 MB (22641030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:dcaaaa3353d40019c34a6311cb6309971b5ebbdaee007a9a2c5c7bdf948c4da5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:e92add0853cca3d90353b7c3ba02856c8fa37ecb63bfc3d8bc2539575ee03eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1087993863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f0831d37aba9bc5d9342e34dcf4211ee421e0c3ad4187b266805c064b550f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:43:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:43:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:43:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:46:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1a884c0500e4a2eccb5a2a364d8d1cdc8c80689d7292e492c144c4dee8f69`  
		Last Modified: Wed, 05 Oct 2022 11:01:16 GMT  
		Size: 97.9 MB (97851974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420841bcfe85d95f042c1930c98a9f177ba6b518fc1c10bd66c341017785ccf5`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 287.9 KB (287858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896c641876dd5da58d9cd9d3b9c73d0a464a3dcb760e5efa747239c51261735`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b4eca3f72bccb69be61064fc7d85e752e7d5c0d0cf14b71a6fe5dea6feb8c`  
		Last Modified: Wed, 05 Oct 2022 11:01:06 GMT  
		Size: 23.2 MB (23226838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c89eceebff238f8a817010c80116db9da5db72367acbeed110da2b63ce962ee`  
		Last Modified: Wed, 05 Oct 2022 11:03:07 GMT  
		Size: 824.8 MB (824815681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:78be1143dc94dd563150a00555027432042e7bf6add3629226596a7999011f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1037757233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9ba2abd3234b7b99a4632f3b505eb02d7129973d39e19be1d45f31ae01566e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:01:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 14:01:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 14:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:04:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2767f80cc9b7f92921da87e086a643d8d80b257ce273716d8795816f765216`  
		Last Modified: Wed, 05 Oct 2022 14:20:48 GMT  
		Size: 95.2 MB (95215484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c34644006693e54ff50141efeaec2467a06586f1f28d4e4874485d96ad999`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 287.8 KB (287799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9377d158c53ca57fb20de69f4e1e1f1bb1741c856365104a808553e58c611ecc`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 2.4 KB (2353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f3f8b1a658efb974ec2a2c92261fc0ca9d5ad9d4eecf003b8752e7b82ab271`  
		Last Modified: Wed, 05 Oct 2022 14:20:38 GMT  
		Size: 22.6 MB (22641030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4de81c13532f2a3ae50f8a84d32f7fbe4788fc88103638857e208cc54f63ef1`  
		Last Modified: Wed, 05 Oct 2022 14:22:40 GMT  
		Size: 782.3 MB (782349387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:dcaaaa3353d40019c34a6311cb6309971b5ebbdaee007a9a2c5c7bdf948c4da5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e92add0853cca3d90353b7c3ba02856c8fa37ecb63bfc3d8bc2539575ee03eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1087993863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f0831d37aba9bc5d9342e34dcf4211ee421e0c3ad4187b266805c064b550f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:43:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:43:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:43:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:46:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1a884c0500e4a2eccb5a2a364d8d1cdc8c80689d7292e492c144c4dee8f69`  
		Last Modified: Wed, 05 Oct 2022 11:01:16 GMT  
		Size: 97.9 MB (97851974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420841bcfe85d95f042c1930c98a9f177ba6b518fc1c10bd66c341017785ccf5`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 287.9 KB (287858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896c641876dd5da58d9cd9d3b9c73d0a464a3dcb760e5efa747239c51261735`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b4eca3f72bccb69be61064fc7d85e752e7d5c0d0cf14b71a6fe5dea6feb8c`  
		Last Modified: Wed, 05 Oct 2022 11:01:06 GMT  
		Size: 23.2 MB (23226838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c89eceebff238f8a817010c80116db9da5db72367acbeed110da2b63ce962ee`  
		Last Modified: Wed, 05 Oct 2022 11:03:07 GMT  
		Size: 824.8 MB (824815681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:78be1143dc94dd563150a00555027432042e7bf6add3629226596a7999011f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1037757233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9ba2abd3234b7b99a4632f3b505eb02d7129973d39e19be1d45f31ae01566e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:01:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 14:01:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 14:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:04:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2767f80cc9b7f92921da87e086a643d8d80b257ce273716d8795816f765216`  
		Last Modified: Wed, 05 Oct 2022 14:20:48 GMT  
		Size: 95.2 MB (95215484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c34644006693e54ff50141efeaec2467a06586f1f28d4e4874485d96ad999`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 287.8 KB (287799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9377d158c53ca57fb20de69f4e1e1f1bb1741c856365104a808553e58c611ecc`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 2.4 KB (2353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f3f8b1a658efb974ec2a2c92261fc0ca9d5ad9d4eecf003b8752e7b82ab271`  
		Last Modified: Wed, 05 Oct 2022 14:20:38 GMT  
		Size: 22.6 MB (22641030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4de81c13532f2a3ae50f8a84d32f7fbe4788fc88103638857e208cc54f63ef1`  
		Last Modified: Wed, 05 Oct 2022 14:22:40 GMT  
		Size: 782.3 MB (782349387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:c2ed7361c46259c8fd1b74efd17eff5ec2610e2376f25c6c178cbb0f455f0153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:0840fe8af38c3bd1f0447f886a73d7896d178e41bc5030948863ad8642c559af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263178182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9edb8205b6372daa73ead068a4158fc78e31fbab557c826bcd3dfd2473dcd91d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:43:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:43:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:43:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1a884c0500e4a2eccb5a2a364d8d1cdc8c80689d7292e492c144c4dee8f69`  
		Last Modified: Wed, 05 Oct 2022 11:01:16 GMT  
		Size: 97.9 MB (97851974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420841bcfe85d95f042c1930c98a9f177ba6b518fc1c10bd66c341017785ccf5`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 287.9 KB (287858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896c641876dd5da58d9cd9d3b9c73d0a464a3dcb760e5efa747239c51261735`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b4eca3f72bccb69be61064fc7d85e752e7d5c0d0cf14b71a6fe5dea6feb8c`  
		Last Modified: Wed, 05 Oct 2022 11:01:06 GMT  
		Size: 23.2 MB (23226838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33669f7bf08ec323d17bd2d63532f30fe9982bbb13f7cf849dd97b000c8a1827
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255407846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be0b50bb3221f9dcf4ace9413a489fa328657908bfeada9464bac70440cca785`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:01:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 14:01:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 14:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2767f80cc9b7f92921da87e086a643d8d80b257ce273716d8795816f765216`  
		Last Modified: Wed, 05 Oct 2022 14:20:48 GMT  
		Size: 95.2 MB (95215484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c34644006693e54ff50141efeaec2467a06586f1f28d4e4874485d96ad999`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 287.8 KB (287799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9377d158c53ca57fb20de69f4e1e1f1bb1741c856365104a808553e58c611ecc`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 2.4 KB (2353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f3f8b1a658efb974ec2a2c92261fc0ca9d5ad9d4eecf003b8752e7b82ab271`  
		Last Modified: Wed, 05 Oct 2022 14:20:38 GMT  
		Size: 22.6 MB (22641030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:c2ed7361c46259c8fd1b74efd17eff5ec2610e2376f25c6c178cbb0f455f0153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:0840fe8af38c3bd1f0447f886a73d7896d178e41bc5030948863ad8642c559af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263178182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9edb8205b6372daa73ead068a4158fc78e31fbab557c826bcd3dfd2473dcd91d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:43:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 10:43:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 10:43:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1a884c0500e4a2eccb5a2a364d8d1cdc8c80689d7292e492c144c4dee8f69`  
		Last Modified: Wed, 05 Oct 2022 11:01:16 GMT  
		Size: 97.9 MB (97851974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420841bcfe85d95f042c1930c98a9f177ba6b518fc1c10bd66c341017785ccf5`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 287.9 KB (287858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896c641876dd5da58d9cd9d3b9c73d0a464a3dcb760e5efa747239c51261735`  
		Last Modified: Wed, 05 Oct 2022 11:01:02 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b4eca3f72bccb69be61064fc7d85e752e7d5c0d0cf14b71a6fe5dea6feb8c`  
		Last Modified: Wed, 05 Oct 2022 11:01:06 GMT  
		Size: 23.2 MB (23226838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33669f7bf08ec323d17bd2d63532f30fe9982bbb13f7cf849dd97b000c8a1827
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255407846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be0b50bb3221f9dcf4ace9413a489fa328657908bfeada9464bac70440cca785`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:01:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Oct 2022 14:01:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 05 Oct 2022 14:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2767f80cc9b7f92921da87e086a643d8d80b257ce273716d8795816f765216`  
		Last Modified: Wed, 05 Oct 2022 14:20:48 GMT  
		Size: 95.2 MB (95215484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c34644006693e54ff50141efeaec2467a06586f1f28d4e4874485d96ad999`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 287.8 KB (287799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9377d158c53ca57fb20de69f4e1e1f1bb1741c856365104a808553e58c611ecc`  
		Last Modified: Wed, 05 Oct 2022 14:20:35 GMT  
		Size: 2.4 KB (2353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f3f8b1a658efb974ec2a2c92261fc0ca9d5ad9d4eecf003b8752e7b82ab271`  
		Last Modified: Wed, 05 Oct 2022 14:20:38 GMT  
		Size: 22.6 MB (22641030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:7cc794ca1e9de0ab8d8391b8f8ae208f73c4be9d3539f8d0dcb1040804d17eff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:13a54ab3b90b8524851f56c52c0461be93b2f50efe05f107fe5da4376ab86df7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141809056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26af6195cf9e62a94108f0efd3276f5333cf3f15a9d422cad76afb79575e01a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:03416f64dcd141aa345f59cfd4dc2d15ac336756d80e80f0077506a039119f9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137261180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ad5a37135505c9a5387b812b23f105dbcd57cb12cf9a764166ed45c8594d86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:7cc794ca1e9de0ab8d8391b8f8ae208f73c4be9d3539f8d0dcb1040804d17eff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:13a54ab3b90b8524851f56c52c0461be93b2f50efe05f107fe5da4376ab86df7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141809056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26af6195cf9e62a94108f0efd3276f5333cf3f15a9d422cad76afb79575e01a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 10:30:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:30:33 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 10:30:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 10:30:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 10:42:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 10:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 10:43:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 10:43:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 10:43:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657ed4bbca2b6e38d245b68fa4e7d8cb04af5f8ce38c735e74ff1efd995ddd2`  
		Last Modified: Wed, 05 Oct 2022 10:57:47 GMT  
		Size: 1.2 MB (1176207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace20a5ecec201be10011eb11e7db7eb3e16a30b7920fb10c049af041ad5ae8f`  
		Last Modified: Wed, 05 Oct 2022 10:57:46 GMT  
		Size: 3.8 MB (3827905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d795fabe79c02ef1562fee456701ad431e78c468d6b007d9022f0ee8f59d1f2`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce660d1b5501b0f6b681547a1cc5bea2b0b3e273fa38be01bd5cd9e602edcea`  
		Last Modified: Wed, 05 Oct 2022 10:57:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e5f6e471571a79c07d753e166119b42b7dffc65e8eb51a2519d6184e69ecb`  
		Last Modified: Wed, 05 Oct 2022 11:00:52 GMT  
		Size: 106.4 MB (106373598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5b83de457e8bad7d32198416bef6f3825171761f6f4e27df9a095e38360f0`  
		Last Modified: Wed, 05 Oct 2022 11:00:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:03416f64dcd141aa345f59cfd4dc2d15ac336756d80e80f0077506a039119f9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137261180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ad5a37135505c9a5387b812b23f105dbcd57cb12cf9a764166ed45c8594d86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:55:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:55:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 05 Oct 2022 13:55:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Oct 2022 13:55:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:55:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Oct 2022 14:00:21 GMT
ENV ROS_DISTRO=rolling
# Wed, 05 Oct 2022 14:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:01:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 05 Oct 2022 14:01:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Oct 2022 14:01:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a891d50162687d5b4db85383705535653c56066b48e0e3314badd3e76d2f8af`  
		Last Modified: Wed, 05 Oct 2022 14:16:45 GMT  
		Size: 1.2 MB (1178125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fc4af9e9380eebc7d111e904fb1098bb4102f7271c19ade184c620ba4d5dc`  
		Last Modified: Wed, 05 Oct 2022 14:16:43 GMT  
		Size: 3.6 MB (3594928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc1176274b8951042f2b29277ebbcdc02bf43ea04b1e95a7e7f80c137ddb1d`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca88c2c17aef59df2c29525001e8bb7f45b3b5e37ef793847df2e89374421e`  
		Last Modified: Wed, 05 Oct 2022 14:16:42 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834504b668bb13d4fcded46b2444690bed0603eccbb71ffd03d0ab432593c8e`  
		Last Modified: Wed, 05 Oct 2022 14:20:23 GMT  
		Size: 104.1 MB (104103500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce9b251482e03203dd3f2b75f07f06ff803e68b582e12a53ce6cc1028c9c58`  
		Last Modified: Wed, 05 Oct 2022 14:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
