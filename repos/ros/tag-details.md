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
$ docker pull ros@sha256:214407db228930d940852cd62493103254a6f3e9c3477474aefc4d97ba20abd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:b4348b200453cad3a5528c25ad14a6e25eae043d3e5528d817c95ceb9aa63fa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250625051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b682ff660f5c81082e60a95563208c394da401a4bc8abca212f1a177d00b5611`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:24:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:24:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476e616a90701bee44fbc310458b18ce75a4bdfe5680a22b27dba9a84bf0ef1c`  
		Last Modified: Tue, 07 Jun 2022 01:50:41 GMT  
		Size: 73.3 MB (73321142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa71ae8a0c62c2ef33328de080cdabeefda3946cc96f59ccad1ecba1796a9209`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 257.1 KB (257124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9ad82940247dc7731be3759d12e58bd52af7b3b53b4731f2d88990db31c281`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0def727ac7744929624ad45072377c38e2b427e4acda1e1c0b108c45e6cae0f`  
		Last Modified: Tue, 07 Jun 2022 01:50:35 GMT  
		Size: 21.7 MB (21663791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c1a3d5daa191f132442b55b8e6f469beb76f9fdbd848838ec22a5ab418217be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226053524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85e77e8b6119016fbb190a1a6cf938b93c9ca5cdd08037ff3c7a5bc2e53ea34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:59:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:59:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:00:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da51ac80ef0bd3a07b16018b52a649d62ec03591a4ca2deb530380c0330f0a44`  
		Last Modified: Tue, 07 Jun 2022 06:21:19 GMT  
		Size: 67.5 MB (67454614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039855e65a5d9a35f11df9edc8607488801249ef521c9a8cb8e9e3be8e492e25`  
		Last Modified: Tue, 07 Jun 2022 06:21:10 GMT  
		Size: 257.1 KB (257142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf578d4ad8db14ff5e85735f040f6db5169e03eae2d6898571946a73e1078a`  
		Last Modified: Tue, 07 Jun 2022 06:21:09 GMT  
		Size: 2.2 KB (2200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce23c0b6803030685f8d276f2f65beef17c9e37a95ce4f0304ca579a92f8901`  
		Last Modified: Tue, 07 Jun 2022 06:21:12 GMT  
		Size: 20.4 MB (20366539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:214407db228930d940852cd62493103254a6f3e9c3477474aefc4d97ba20abd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b4348b200453cad3a5528c25ad14a6e25eae043d3e5528d817c95ceb9aa63fa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250625051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b682ff660f5c81082e60a95563208c394da401a4bc8abca212f1a177d00b5611`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:24:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:24:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476e616a90701bee44fbc310458b18ce75a4bdfe5680a22b27dba9a84bf0ef1c`  
		Last Modified: Tue, 07 Jun 2022 01:50:41 GMT  
		Size: 73.3 MB (73321142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa71ae8a0c62c2ef33328de080cdabeefda3946cc96f59ccad1ecba1796a9209`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 257.1 KB (257124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9ad82940247dc7731be3759d12e58bd52af7b3b53b4731f2d88990db31c281`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0def727ac7744929624ad45072377c38e2b427e4acda1e1c0b108c45e6cae0f`  
		Last Modified: Tue, 07 Jun 2022 01:50:35 GMT  
		Size: 21.7 MB (21663791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c1a3d5daa191f132442b55b8e6f469beb76f9fdbd848838ec22a5ab418217be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226053524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85e77e8b6119016fbb190a1a6cf938b93c9ca5cdd08037ff3c7a5bc2e53ea34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:59:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:59:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:00:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da51ac80ef0bd3a07b16018b52a649d62ec03591a4ca2deb530380c0330f0a44`  
		Last Modified: Tue, 07 Jun 2022 06:21:19 GMT  
		Size: 67.5 MB (67454614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039855e65a5d9a35f11df9edc8607488801249ef521c9a8cb8e9e3be8e492e25`  
		Last Modified: Tue, 07 Jun 2022 06:21:10 GMT  
		Size: 257.1 KB (257142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf578d4ad8db14ff5e85735f040f6db5169e03eae2d6898571946a73e1078a`  
		Last Modified: Tue, 07 Jun 2022 06:21:09 GMT  
		Size: 2.2 KB (2200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce23c0b6803030685f8d276f2f65beef17c9e37a95ce4f0304ca579a92f8901`  
		Last Modified: Tue, 07 Jun 2022 06:21:12 GMT  
		Size: 20.4 MB (20366539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:214407db228930d940852cd62493103254a6f3e9c3477474aefc4d97ba20abd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:b4348b200453cad3a5528c25ad14a6e25eae043d3e5528d817c95ceb9aa63fa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250625051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b682ff660f5c81082e60a95563208c394da401a4bc8abca212f1a177d00b5611`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:24:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:24:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476e616a90701bee44fbc310458b18ce75a4bdfe5680a22b27dba9a84bf0ef1c`  
		Last Modified: Tue, 07 Jun 2022 01:50:41 GMT  
		Size: 73.3 MB (73321142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa71ae8a0c62c2ef33328de080cdabeefda3946cc96f59ccad1ecba1796a9209`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 257.1 KB (257124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9ad82940247dc7731be3759d12e58bd52af7b3b53b4731f2d88990db31c281`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0def727ac7744929624ad45072377c38e2b427e4acda1e1c0b108c45e6cae0f`  
		Last Modified: Tue, 07 Jun 2022 01:50:35 GMT  
		Size: 21.7 MB (21663791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c1a3d5daa191f132442b55b8e6f469beb76f9fdbd848838ec22a5ab418217be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226053524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85e77e8b6119016fbb190a1a6cf938b93c9ca5cdd08037ff3c7a5bc2e53ea34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:59:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:59:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:00:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da51ac80ef0bd3a07b16018b52a649d62ec03591a4ca2deb530380c0330f0a44`  
		Last Modified: Tue, 07 Jun 2022 06:21:19 GMT  
		Size: 67.5 MB (67454614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039855e65a5d9a35f11df9edc8607488801249ef521c9a8cb8e9e3be8e492e25`  
		Last Modified: Tue, 07 Jun 2022 06:21:10 GMT  
		Size: 257.1 KB (257142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf578d4ad8db14ff5e85735f040f6db5169e03eae2d6898571946a73e1078a`  
		Last Modified: Tue, 07 Jun 2022 06:21:09 GMT  
		Size: 2.2 KB (2200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce23c0b6803030685f8d276f2f65beef17c9e37a95ce4f0304ca579a92f8901`  
		Last Modified: Tue, 07 Jun 2022 06:21:12 GMT  
		Size: 20.4 MB (20366539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:7df192364c54a873cad7e6b7589d66660803a5ec19a0d087712851af92d5e77d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f15a09d011219100f61223fe24f0f4089363c0ba26deded9377a14c02e82e233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155380712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09673a05a28a9b49672b353d9cfd3f5cb2b1423ba45f7ad47fcb0326878b002a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d4e1245fc3f2b696553eb4860a79b6453c6b3581ca7369a1b120b81bdc2e4ee8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137973029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5beee1c47df5e0f5233fd81c9c3919708af3ec9e1ea72feae0995d230006e1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:7df192364c54a873cad7e6b7589d66660803a5ec19a0d087712851af92d5e77d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:f15a09d011219100f61223fe24f0f4089363c0ba26deded9377a14c02e82e233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155380712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09673a05a28a9b49672b353d9cfd3f5cb2b1423ba45f7ad47fcb0326878b002a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d4e1245fc3f2b696553eb4860a79b6453c6b3581ca7369a1b120b81bdc2e4ee8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137973029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5beee1c47df5e0f5233fd81c9c3919708af3ec9e1ea72feae0995d230006e1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:dfcdbfc5622005e48a57a28c840bd8256695f9c52aad78e6906d3049044fd292
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:845fc60bb1307a03bf649f02283e0cfe1304fbf4823b8541fb1a0060c543b43f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348478447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665532b112476db2c919c9d6ea566b426ee92be833f5eb901fff3e427584f343`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:24:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:24:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:25:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:25:00 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 01:25:00 GMT
ENV ROS2_DISTRO=foxy
# Tue, 07 Jun 2022 01:25:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:25:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:25:38 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476e616a90701bee44fbc310458b18ce75a4bdfe5680a22b27dba9a84bf0ef1c`  
		Last Modified: Tue, 07 Jun 2022 01:50:41 GMT  
		Size: 73.3 MB (73321142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa71ae8a0c62c2ef33328de080cdabeefda3946cc96f59ccad1ecba1796a9209`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 257.1 KB (257124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9ad82940247dc7731be3759d12e58bd52af7b3b53b4731f2d88990db31c281`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0def727ac7744929624ad45072377c38e2b427e4acda1e1c0b108c45e6cae0f`  
		Last Modified: Tue, 07 Jun 2022 01:50:35 GMT  
		Size: 21.7 MB (21663791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3d2bc7757d3d9d4bb3b8f6a36ae62da3d95745ee4f11a56e38fdf554486938`  
		Last Modified: Tue, 07 Jun 2022 01:50:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ebc1131df0b50eabcf4d4c6f3247f87ddbbffc13edbfa443427e13add36ad4`  
		Last Modified: Tue, 07 Jun 2022 01:50:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12074399c950505a578a1947414ca27201fa77d5d64a7acd791e9a54957a4f68`  
		Last Modified: Tue, 07 Jun 2022 01:51:10 GMT  
		Size: 76.3 MB (76316167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4199ae2cdec8ea37d6ec3ae7cdeab825069a3f7d924bb5cbea0c4a5dc8f65`  
		Last Modified: Tue, 07 Jun 2022 01:51:00 GMT  
		Size: 21.5 MB (21536602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4fe45deb83c6b2ef4410607491f98ec61e82e32dde9b31b45a8868a4fc9248`  
		Last Modified: Tue, 07 Jun 2022 01:50:55 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9fa283c8598fc76684226b6f65b836c00b9d130696533bf623845110a5b71027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 MB (316167892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2baa20aae39af9039e05f17398914fe7dfa6e7c6d4496da5a250957c69e6c245`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:59:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:59:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:00:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:00:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 06:00:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:00:28 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 06:00:30 GMT
ENV ROS2_DISTRO=foxy
# Tue, 07 Jun 2022 06:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:01:14 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da51ac80ef0bd3a07b16018b52a649d62ec03591a4ca2deb530380c0330f0a44`  
		Last Modified: Tue, 07 Jun 2022 06:21:19 GMT  
		Size: 67.5 MB (67454614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039855e65a5d9a35f11df9edc8607488801249ef521c9a8cb8e9e3be8e492e25`  
		Last Modified: Tue, 07 Jun 2022 06:21:10 GMT  
		Size: 257.1 KB (257142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf578d4ad8db14ff5e85735f040f6db5169e03eae2d6898571946a73e1078a`  
		Last Modified: Tue, 07 Jun 2022 06:21:09 GMT  
		Size: 2.2 KB (2200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce23c0b6803030685f8d276f2f65beef17c9e37a95ce4f0304ca579a92f8901`  
		Last Modified: Tue, 07 Jun 2022 06:21:12 GMT  
		Size: 20.4 MB (20366539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3217c1f4b754041ab2f4260ac2ddf77be53a7318d99d8539e26d73b86a872f`  
		Last Modified: Tue, 07 Jun 2022 06:21:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b3b3a7dd0b783eab2421ff96b00d4bf25eb41057a27a39f1f4a90174f1fbc`  
		Last Modified: Tue, 07 Jun 2022 06:21:49 GMT  
		Size: 76.2 MB (76156799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b38386e8040edbd93e865cbc03188975712bce21f1fb727cc3ecd02f255bf3`  
		Last Modified: Tue, 07 Jun 2022 06:21:37 GMT  
		Size: 14.0 MB (13957100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d63e2111fa8780ea446d84d204450a96516d1d076b93e8a4b0a48684463fe1a`  
		Last Modified: Tue, 07 Jun 2022 06:21:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:dfcdbfc5622005e48a57a28c840bd8256695f9c52aad78e6906d3049044fd292
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:845fc60bb1307a03bf649f02283e0cfe1304fbf4823b8541fb1a0060c543b43f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348478447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665532b112476db2c919c9d6ea566b426ee92be833f5eb901fff3e427584f343`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:23:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:23:54 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:24:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:24:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:24:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:25:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:25:00 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 01:25:00 GMT
ENV ROS2_DISTRO=foxy
# Tue, 07 Jun 2022 01:25:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:25:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:25:38 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42810f84e69169e13f4ba7e14a1a7fa6d81dba996d2b091493577783be695e`  
		Last Modified: Tue, 07 Jun 2022 01:50:21 GMT  
		Size: 120.1 MB (120077388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f92457a493c04a77f0ac61cd065d158768a70191e86bf92fc446076123f8e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476e616a90701bee44fbc310458b18ce75a4bdfe5680a22b27dba9a84bf0ef1c`  
		Last Modified: Tue, 07 Jun 2022 01:50:41 GMT  
		Size: 73.3 MB (73321142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa71ae8a0c62c2ef33328de080cdabeefda3946cc96f59ccad1ecba1796a9209`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 257.1 KB (257124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9ad82940247dc7731be3759d12e58bd52af7b3b53b4731f2d88990db31c281`  
		Last Modified: Tue, 07 Jun 2022 01:50:31 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0def727ac7744929624ad45072377c38e2b427e4acda1e1c0b108c45e6cae0f`  
		Last Modified: Tue, 07 Jun 2022 01:50:35 GMT  
		Size: 21.7 MB (21663791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3d2bc7757d3d9d4bb3b8f6a36ae62da3d95745ee4f11a56e38fdf554486938`  
		Last Modified: Tue, 07 Jun 2022 01:50:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ebc1131df0b50eabcf4d4c6f3247f87ddbbffc13edbfa443427e13add36ad4`  
		Last Modified: Tue, 07 Jun 2022 01:50:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12074399c950505a578a1947414ca27201fa77d5d64a7acd791e9a54957a4f68`  
		Last Modified: Tue, 07 Jun 2022 01:51:10 GMT  
		Size: 76.3 MB (76316167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4199ae2cdec8ea37d6ec3ae7cdeab825069a3f7d924bb5cbea0c4a5dc8f65`  
		Last Modified: Tue, 07 Jun 2022 01:51:00 GMT  
		Size: 21.5 MB (21536602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4fe45deb83c6b2ef4410607491f98ec61e82e32dde9b31b45a8868a4fc9248`  
		Last Modified: Tue, 07 Jun 2022 01:50:55 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9fa283c8598fc76684226b6f65b836c00b9d130696533bf623845110a5b71027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 MB (316167892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2baa20aae39af9039e05f17398914fe7dfa6e7c6d4496da5a250957c69e6c245`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 05:59:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:59:13 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:59:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:59:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:59:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:00:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:00:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 06:00:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:00:28 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 06:00:30 GMT
ENV ROS2_DISTRO=foxy
# Tue, 07 Jun 2022 06:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:01:14 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3959e0f6ed1971e7ada61486d677ef1ae06a0844bb1f91bc5cace3e398a9a`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da51ac80ef0bd3a07b16018b52a649d62ec03591a4ca2deb530380c0330f0a44`  
		Last Modified: Tue, 07 Jun 2022 06:21:19 GMT  
		Size: 67.5 MB (67454614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039855e65a5d9a35f11df9edc8607488801249ef521c9a8cb8e9e3be8e492e25`  
		Last Modified: Tue, 07 Jun 2022 06:21:10 GMT  
		Size: 257.1 KB (257142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf578d4ad8db14ff5e85735f040f6db5169e03eae2d6898571946a73e1078a`  
		Last Modified: Tue, 07 Jun 2022 06:21:09 GMT  
		Size: 2.2 KB (2200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce23c0b6803030685f8d276f2f65beef17c9e37a95ce4f0304ca579a92f8901`  
		Last Modified: Tue, 07 Jun 2022 06:21:12 GMT  
		Size: 20.4 MB (20366539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3217c1f4b754041ab2f4260ac2ddf77be53a7318d99d8539e26d73b86a872f`  
		Last Modified: Tue, 07 Jun 2022 06:21:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b3b3a7dd0b783eab2421ff96b00d4bf25eb41057a27a39f1f4a90174f1fbc`  
		Last Modified: Tue, 07 Jun 2022 06:21:49 GMT  
		Size: 76.2 MB (76156799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b38386e8040edbd93e865cbc03188975712bce21f1fb727cc3ecd02f255bf3`  
		Last Modified: Tue, 07 Jun 2022 06:21:37 GMT  
		Size: 14.0 MB (13957100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d63e2111fa8780ea446d84d204450a96516d1d076b93e8a4b0a48684463fe1a`  
		Last Modified: Tue, 07 Jun 2022 06:21:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:8c224b774d3f2070a9a48807706b160c0f87f27402f62518df3b6941b221ce69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:8c82d0660739d6c52223a9cf005975487e30e6591c506ddbc980d8d61308176c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234881597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c8e7e5b1cfcf97b62539c8421b12d3ff5277d5a997478751d1803df612bce`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:26:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:27:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9cacbf113eab2c035d8ce7928a9dc392a930695e0d6675b68fa369e4f25a36`  
		Last Modified: Tue, 07 Jun 2022 01:51:59 GMT  
		Size: 73.3 MB (73277330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720d00ff5b5e945d87052fda142a10225f078857510d58daf3cb774dd7cf2409`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 268.7 KB (268680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5088eaefe4d16e72f6bbad02947f97b7bf3fb5f630d81bf115b23b58112b6a`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 2.3 KB (2252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32c58c406e4f680586936ef1737a7f1951158628d31bd2aa082b331677f7f7c`  
		Last Modified: Tue, 07 Jun 2022 01:51:52 GMT  
		Size: 22.1 MB (22133376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:578143df77fa24524ab61f80d3d2cccfeae8b88b80a5a2d47fcd7920fa8e68e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223121508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d2b07db6013b57e31dcfc9b83b76a1db0f3678ce86b35eb4265f40bf5a81926`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:02:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:02:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdb738ca32d002eb3ccc2390bd9947b973ebea1e2c458a6547b8667cfbff47`  
		Last Modified: Tue, 07 Jun 2022 06:22:38 GMT  
		Size: 67.4 MB (67398488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81030be58777c96d8770d3770d1d9b2522fd0711886691af9d18cca52cb14ee8`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 268.6 KB (268614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ee83f98b9818c719b7d9bf9d9ba032ccb657524a1b686e9aa2b72338b28f7`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d548d4dc4acdc321e91080b8f09593a4a7dfebd470ed65352dc5360a7a90ee5`  
		Last Modified: Tue, 07 Jun 2022 06:22:32 GMT  
		Size: 21.5 MB (21453703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:8c224b774d3f2070a9a48807706b160c0f87f27402f62518df3b6941b221ce69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8c82d0660739d6c52223a9cf005975487e30e6591c506ddbc980d8d61308176c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234881597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c8e7e5b1cfcf97b62539c8421b12d3ff5277d5a997478751d1803df612bce`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:26:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:27:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9cacbf113eab2c035d8ce7928a9dc392a930695e0d6675b68fa369e4f25a36`  
		Last Modified: Tue, 07 Jun 2022 01:51:59 GMT  
		Size: 73.3 MB (73277330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720d00ff5b5e945d87052fda142a10225f078857510d58daf3cb774dd7cf2409`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 268.7 KB (268680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5088eaefe4d16e72f6bbad02947f97b7bf3fb5f630d81bf115b23b58112b6a`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 2.3 KB (2252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32c58c406e4f680586936ef1737a7f1951158628d31bd2aa082b331677f7f7c`  
		Last Modified: Tue, 07 Jun 2022 01:51:52 GMT  
		Size: 22.1 MB (22133376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:578143df77fa24524ab61f80d3d2cccfeae8b88b80a5a2d47fcd7920fa8e68e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223121508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d2b07db6013b57e31dcfc9b83b76a1db0f3678ce86b35eb4265f40bf5a81926`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:02:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:02:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdb738ca32d002eb3ccc2390bd9947b973ebea1e2c458a6547b8667cfbff47`  
		Last Modified: Tue, 07 Jun 2022 06:22:38 GMT  
		Size: 67.4 MB (67398488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81030be58777c96d8770d3770d1d9b2522fd0711886691af9d18cca52cb14ee8`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 268.6 KB (268614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ee83f98b9818c719b7d9bf9d9ba032ccb657524a1b686e9aa2b72338b28f7`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d548d4dc4acdc321e91080b8f09593a4a7dfebd470ed65352dc5360a7a90ee5`  
		Last Modified: Tue, 07 Jun 2022 06:22:32 GMT  
		Size: 21.5 MB (21453703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:8c224b774d3f2070a9a48807706b160c0f87f27402f62518df3b6941b221ce69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:8c82d0660739d6c52223a9cf005975487e30e6591c506ddbc980d8d61308176c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234881597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c8e7e5b1cfcf97b62539c8421b12d3ff5277d5a997478751d1803df612bce`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:26:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:27:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9cacbf113eab2c035d8ce7928a9dc392a930695e0d6675b68fa369e4f25a36`  
		Last Modified: Tue, 07 Jun 2022 01:51:59 GMT  
		Size: 73.3 MB (73277330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720d00ff5b5e945d87052fda142a10225f078857510d58daf3cb774dd7cf2409`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 268.7 KB (268680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5088eaefe4d16e72f6bbad02947f97b7bf3fb5f630d81bf115b23b58112b6a`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 2.3 KB (2252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32c58c406e4f680586936ef1737a7f1951158628d31bd2aa082b331677f7f7c`  
		Last Modified: Tue, 07 Jun 2022 01:51:52 GMT  
		Size: 22.1 MB (22133376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:578143df77fa24524ab61f80d3d2cccfeae8b88b80a5a2d47fcd7920fa8e68e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223121508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d2b07db6013b57e31dcfc9b83b76a1db0f3678ce86b35eb4265f40bf5a81926`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:02:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:02:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdb738ca32d002eb3ccc2390bd9947b973ebea1e2c458a6547b8667cfbff47`  
		Last Modified: Tue, 07 Jun 2022 06:22:38 GMT  
		Size: 67.4 MB (67398488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81030be58777c96d8770d3770d1d9b2522fd0711886691af9d18cca52cb14ee8`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 268.6 KB (268614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ee83f98b9818c719b7d9bf9d9ba032ccb657524a1b686e9aa2b72338b28f7`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d548d4dc4acdc321e91080b8f09593a4a7dfebd470ed65352dc5360a7a90ee5`  
		Last Modified: Tue, 07 Jun 2022 06:22:32 GMT  
		Size: 21.5 MB (21453703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:615680e2fb0351007b3b8717d2477006cbc3e4b629e5de583b88f55e1ae81ebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:0e7c5508145907219100d730b3e2ee0f98ca57c4227c88bcff8c2c31d5888b88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139199959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f911775cb8c5f85340bcc74008e82a5a401fe73db96840f2d35bfec213252e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ab343f933f6b7065473269eb7c5638c4d4bb7c26a88b17630eb0bae032f90605
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133998522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70723caba7a3ed285e0cfae6bebc3632b07de8131b526e33726772d9e7a6a167`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:615680e2fb0351007b3b8717d2477006cbc3e4b629e5de583b88f55e1ae81ebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:0e7c5508145907219100d730b3e2ee0f98ca57c4227c88bcff8c2c31d5888b88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139199959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f911775cb8c5f85340bcc74008e82a5a401fe73db96840f2d35bfec213252e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ab343f933f6b7065473269eb7c5638c4d4bb7c26a88b17630eb0bae032f90605
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133998522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70723caba7a3ed285e0cfae6bebc3632b07de8131b526e33726772d9e7a6a167`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:0f5768036dcccfa4111e08a7c4f019799e948a6d5aa3000329d22b4e9d0f23db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:1c71f11e6734d6f5f8e01f148ecc8f0475e2b348ce251dc18dbe0c3040351a5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329937165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b8ad841d315f200b9a88d6426193aa1b2fd23935cceb636c50f76969baa596`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:26:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:27:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:27:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:27:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:27:25 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 01:27:25 GMT
ENV ROS2_DISTRO=galactic
# Tue, 07 Jun 2022 01:27:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:02 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9cacbf113eab2c035d8ce7928a9dc392a930695e0d6675b68fa369e4f25a36`  
		Last Modified: Tue, 07 Jun 2022 01:51:59 GMT  
		Size: 73.3 MB (73277330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720d00ff5b5e945d87052fda142a10225f078857510d58daf3cb774dd7cf2409`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 268.7 KB (268680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5088eaefe4d16e72f6bbad02947f97b7bf3fb5f630d81bf115b23b58112b6a`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 2.3 KB (2252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32c58c406e4f680586936ef1737a7f1951158628d31bd2aa082b331677f7f7c`  
		Last Modified: Tue, 07 Jun 2022 01:51:52 GMT  
		Size: 22.1 MB (22133376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6de3057fa64b56f8fd78bfbbac13a43f555a9032f185ea6c74b317bde0c5bff`  
		Last Modified: Tue, 07 Jun 2022 01:52:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e366d993dbd82b7298b67fa2cf4372e71e782e237c5e0fdf33754c5c464ed8c4`  
		Last Modified: Tue, 07 Jun 2022 01:52:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2734507aac8887f100fa76bc1d892e7ad3bbc5f1eca6c412b9865484a23e172`  
		Last Modified: Tue, 07 Jun 2022 01:52:27 GMT  
		Size: 78.6 MB (78590861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0b49439b21162a676f3301adeab1d6e0747ad9c793a002290624bb76ec1cab`  
		Last Modified: Tue, 07 Jun 2022 01:52:16 GMT  
		Size: 16.5 MB (16464080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95fcf7655c800415f2cd300c5a93dfe261d2ca3d3500cfa5ddf8bc14ebdd7e`  
		Last Modified: Tue, 07 Jun 2022 01:52:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:de8cecf51194c65cb6f05318796953002ba6778bee1380fc4ee5943d058d2d9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317223401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681be6f9720446985d56095e0821dcf3b9fb65b0d4e7c098de155b20453ef637`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:02:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:02:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:03:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 06:03:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:03:32 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 06:03:33 GMT
ENV ROS2_DISTRO=galactic
# Tue, 07 Jun 2022 06:04:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:29 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdb738ca32d002eb3ccc2390bd9947b973ebea1e2c458a6547b8667cfbff47`  
		Last Modified: Tue, 07 Jun 2022 06:22:38 GMT  
		Size: 67.4 MB (67398488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81030be58777c96d8770d3770d1d9b2522fd0711886691af9d18cca52cb14ee8`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 268.6 KB (268614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ee83f98b9818c719b7d9bf9d9ba032ccb657524a1b686e9aa2b72338b28f7`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d548d4dc4acdc321e91080b8f09593a4a7dfebd470ed65352dc5360a7a90ee5`  
		Last Modified: Tue, 07 Jun 2022 06:22:32 GMT  
		Size: 21.5 MB (21453703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732118f6f3cf826dd5af9cb2bffd86f401926e2ff377d2f508afb53f8d663ca5`  
		Last Modified: Tue, 07 Jun 2022 06:22:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a257cf0c11cdf31695455adfdfb172143fa9fa5b5d9df59e0b367d11d42c52d4`  
		Last Modified: Tue, 07 Jun 2022 06:23:08 GMT  
		Size: 78.3 MB (78339763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d568e04a37adaf6818198dac4a6cef595712bb0d7222c0ecf0e0dab16e3df2`  
		Last Modified: Tue, 07 Jun 2022 06:22:56 GMT  
		Size: 15.8 MB (15761659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23314d7ca45436a7765150fdc004ae7b8ceab31e976f471f25265d37702f661`  
		Last Modified: Tue, 07 Jun 2022 06:22:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:0f5768036dcccfa4111e08a7c4f019799e948a6d5aa3000329d22b4e9d0f23db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:1c71f11e6734d6f5f8e01f148ecc8f0475e2b348ce251dc18dbe0c3040351a5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329937165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b8ad841d315f200b9a88d6426193aa1b2fd23935cceb636c50f76969baa596`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:22:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:25:47 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:26:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:26:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:26:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:26:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:27:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:27:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:27:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:27:25 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 01:27:25 GMT
ENV ROS2_DISTRO=galactic
# Tue, 07 Jun 2022 01:27:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:02 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f29772f338ee6a1336a8cfeab6d4550be032d0e9cea76c782ba25f708e14a6`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699c33a19954e95275906408065472c7989f2a8bc685a5c9ffc5f7a70446e7`  
		Last Modified: Tue, 07 Jun 2022 01:50:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2866cb0f0d4336034617ceab231c79373943a15649ab70ecefc8de2e91f27`  
		Last Modified: Tue, 07 Jun 2022 01:51:37 GMT  
		Size: 103.9 MB (103896635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5a4ca68185ef75652d1ca68dc20ca1491b8e12c347cf48db6af2b5441aeb2`  
		Last Modified: Tue, 07 Jun 2022 01:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9cacbf113eab2c035d8ce7928a9dc392a930695e0d6675b68fa369e4f25a36`  
		Last Modified: Tue, 07 Jun 2022 01:51:59 GMT  
		Size: 73.3 MB (73277330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720d00ff5b5e945d87052fda142a10225f078857510d58daf3cb774dd7cf2409`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 268.7 KB (268680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5088eaefe4d16e72f6bbad02947f97b7bf3fb5f630d81bf115b23b58112b6a`  
		Last Modified: Tue, 07 Jun 2022 01:51:48 GMT  
		Size: 2.3 KB (2252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32c58c406e4f680586936ef1737a7f1951158628d31bd2aa082b331677f7f7c`  
		Last Modified: Tue, 07 Jun 2022 01:51:52 GMT  
		Size: 22.1 MB (22133376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6de3057fa64b56f8fd78bfbbac13a43f555a9032f185ea6c74b317bde0c5bff`  
		Last Modified: Tue, 07 Jun 2022 01:52:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e366d993dbd82b7298b67fa2cf4372e71e782e237c5e0fdf33754c5c464ed8c4`  
		Last Modified: Tue, 07 Jun 2022 01:52:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2734507aac8887f100fa76bc1d892e7ad3bbc5f1eca6c412b9865484a23e172`  
		Last Modified: Tue, 07 Jun 2022 01:52:27 GMT  
		Size: 78.6 MB (78590861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0b49439b21162a676f3301adeab1d6e0747ad9c793a002290624bb76ec1cab`  
		Last Modified: Tue, 07 Jun 2022 01:52:16 GMT  
		Size: 16.5 MB (16464080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95fcf7655c800415f2cd300c5a93dfe261d2ca3d3500cfa5ddf8bc14ebdd7e`  
		Last Modified: Tue, 07 Jun 2022 01:52:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:de8cecf51194c65cb6f05318796953002ba6778bee1380fc4ee5943d058d2d9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317223401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681be6f9720446985d56095e0821dcf3b9fb65b0d4e7c098de155b20453ef637`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:02:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:02:15 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:02:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:02:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:03:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 06:03:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:03:32 GMT
ENV ROS1_DISTRO=noetic
# Tue, 07 Jun 2022 06:03:33 GMT
ENV ROS2_DISTRO=galactic
# Tue, 07 Jun 2022 06:04:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:29 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d097227b67efe3e83968a3b510871a9e6c5ea1593bfc39f5658f5df770aaf4dd`  
		Last Modified: Tue, 07 Jun 2022 06:22:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdb738ca32d002eb3ccc2390bd9947b973ebea1e2c458a6547b8667cfbff47`  
		Last Modified: Tue, 07 Jun 2022 06:22:38 GMT  
		Size: 67.4 MB (67398488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81030be58777c96d8770d3770d1d9b2522fd0711886691af9d18cca52cb14ee8`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 268.6 KB (268614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ee83f98b9818c719b7d9bf9d9ba032ccb657524a1b686e9aa2b72338b28f7`  
		Last Modified: Tue, 07 Jun 2022 06:22:29 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d548d4dc4acdc321e91080b8f09593a4a7dfebd470ed65352dc5360a7a90ee5`  
		Last Modified: Tue, 07 Jun 2022 06:22:32 GMT  
		Size: 21.5 MB (21453703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732118f6f3cf826dd5af9cb2bffd86f401926e2ff377d2f508afb53f8d663ca5`  
		Last Modified: Tue, 07 Jun 2022 06:22:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a257cf0c11cdf31695455adfdfb172143fa9fa5b5d9df59e0b367d11d42c52d4`  
		Last Modified: Tue, 07 Jun 2022 06:23:08 GMT  
		Size: 78.3 MB (78339763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d568e04a37adaf6818198dac4a6cef595712bb0d7222c0ecf0e0dab16e3df2`  
		Last Modified: Tue, 07 Jun 2022 06:22:56 GMT  
		Size: 15.8 MB (15761659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23314d7ca45436a7765150fdc004ae7b8ceab31e976f471f25265d37702f661`  
		Last Modified: Tue, 07 Jun 2022 06:22:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:4d776d805039fa1a17b7ad2d3af4860bb4b861ad0f68b0e315267c36a40576f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:e0e17b700196408888ab48ab7c914db7819ee82f326f2ba2cb6f8fe6d75f4919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262693307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f0adf022ed5d398f0b7f1dbd93f0daf5c2c99f625fc0225a710c59afc1ed1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:31:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:31:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f9c0d1c45afeb74327e597df16894662a900d8c355992eefeeb675d0769066`  
		Last Modified: Tue, 07 Jun 2022 01:53:18 GMT  
		Size: 97.8 MB (97838689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14416f74a08632618c2f5b301b40e1537c737981626b6d5a308c05ac0685cc69`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 275.5 KB (275465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02f37a74d93c667b726c4a1db0b1e11226232ac78f437a285603c07d13d92ca`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53e3e8d33911936f4e2551e3eae9526aa1994e89d0d66c3c0459900bd6d68ba`  
		Last Modified: Tue, 07 Jun 2022 01:53:08 GMT  
		Size: 23.0 MB (23007607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ccc3162be85ff1fa70519bfd257628a728e005b197bf1012a9f11ce2b98cff52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254957822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101c0763c9519ba7c8cae58c6684c706c6ef29b278b56091400ab961143e8f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:06:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:06:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:06:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3035c9ae316d5f3965a292003ea9a80fe4752179a91c4017aa9b0d68e07e6`  
		Last Modified: Tue, 07 Jun 2022 06:24:00 GMT  
		Size: 95.2 MB (95223955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e084c9022832d9836eeda7d8e74c887675c25779e5a393fa13d00d7346d01803`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 275.4 KB (275402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58093b060a5da797812c0b09b2a2da2dbd1417c61297bc1c8d05a88397fb4bf2`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1fdae332ebe53c9728d99ef659e2e4b56a11492df80326566359654277d7ff`  
		Last Modified: Tue, 07 Jun 2022 06:23:50 GMT  
		Size: 22.4 MB (22425056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:44fd9939010e89bd49d44fb80879eaf129796d6972c7cee17f2598c151e958d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:27483c4fcbd0c30e7ebab8fbcb40082afec16ee5b6315039a2cde3775340d883
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1089350167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb421c82f61f4ddcb96ad27e58f55f19f2e80c5085cb95fcb6ce621276f5d4e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:31:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:31:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f9c0d1c45afeb74327e597df16894662a900d8c355992eefeeb675d0769066`  
		Last Modified: Tue, 07 Jun 2022 01:53:18 GMT  
		Size: 97.8 MB (97838689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14416f74a08632618c2f5b301b40e1537c737981626b6d5a308c05ac0685cc69`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 275.5 KB (275465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02f37a74d93c667b726c4a1db0b1e11226232ac78f437a285603c07d13d92ca`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53e3e8d33911936f4e2551e3eae9526aa1994e89d0d66c3c0459900bd6d68ba`  
		Last Modified: Tue, 07 Jun 2022 01:53:08 GMT  
		Size: 23.0 MB (23007607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20deccde8fa8f294f08a191be290ab9722313f3ef8082023a2edd484a942e2e2`  
		Last Modified: Tue, 07 Jun 2022 01:55:14 GMT  
		Size: 826.7 MB (826656860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d8afd59ce4616aa83adab63232ba9f967dd0022e3462b8d5ac64563bd33e955f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034054900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c8ad492ece589b27428132478ef03d4a1bb3575506fbd508d2950d592adc1b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:06:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:06:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:06:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:09:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3035c9ae316d5f3965a292003ea9a80fe4752179a91c4017aa9b0d68e07e6`  
		Last Modified: Tue, 07 Jun 2022 06:24:00 GMT  
		Size: 95.2 MB (95223955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e084c9022832d9836eeda7d8e74c887675c25779e5a393fa13d00d7346d01803`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 275.4 KB (275402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58093b060a5da797812c0b09b2a2da2dbd1417c61297bc1c8d05a88397fb4bf2`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1fdae332ebe53c9728d99ef659e2e4b56a11492df80326566359654277d7ff`  
		Last Modified: Tue, 07 Jun 2022 06:23:50 GMT  
		Size: 22.4 MB (22425056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1139d34e8c59a50685ff78ebbb1af9081ed86662e4bfb59b75c5f2cc509cdeb5`  
		Last Modified: Tue, 07 Jun 2022 06:25:52 GMT  
		Size: 779.1 MB (779097078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:44fd9939010e89bd49d44fb80879eaf129796d6972c7cee17f2598c151e958d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:27483c4fcbd0c30e7ebab8fbcb40082afec16ee5b6315039a2cde3775340d883
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1089350167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb421c82f61f4ddcb96ad27e58f55f19f2e80c5085cb95fcb6ce621276f5d4e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:31:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:31:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f9c0d1c45afeb74327e597df16894662a900d8c355992eefeeb675d0769066`  
		Last Modified: Tue, 07 Jun 2022 01:53:18 GMT  
		Size: 97.8 MB (97838689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14416f74a08632618c2f5b301b40e1537c737981626b6d5a308c05ac0685cc69`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 275.5 KB (275465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02f37a74d93c667b726c4a1db0b1e11226232ac78f437a285603c07d13d92ca`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53e3e8d33911936f4e2551e3eae9526aa1994e89d0d66c3c0459900bd6d68ba`  
		Last Modified: Tue, 07 Jun 2022 01:53:08 GMT  
		Size: 23.0 MB (23007607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20deccde8fa8f294f08a191be290ab9722313f3ef8082023a2edd484a942e2e2`  
		Last Modified: Tue, 07 Jun 2022 01:55:14 GMT  
		Size: 826.7 MB (826656860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d8afd59ce4616aa83adab63232ba9f967dd0022e3462b8d5ac64563bd33e955f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034054900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c8ad492ece589b27428132478ef03d4a1bb3575506fbd508d2950d592adc1b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:06:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:06:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:06:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:09:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3035c9ae316d5f3965a292003ea9a80fe4752179a91c4017aa9b0d68e07e6`  
		Last Modified: Tue, 07 Jun 2022 06:24:00 GMT  
		Size: 95.2 MB (95223955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e084c9022832d9836eeda7d8e74c887675c25779e5a393fa13d00d7346d01803`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 275.4 KB (275402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58093b060a5da797812c0b09b2a2da2dbd1417c61297bc1c8d05a88397fb4bf2`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1fdae332ebe53c9728d99ef659e2e4b56a11492df80326566359654277d7ff`  
		Last Modified: Tue, 07 Jun 2022 06:23:50 GMT  
		Size: 22.4 MB (22425056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1139d34e8c59a50685ff78ebbb1af9081ed86662e4bfb59b75c5f2cc509cdeb5`  
		Last Modified: Tue, 07 Jun 2022 06:25:52 GMT  
		Size: 779.1 MB (779097078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:4d776d805039fa1a17b7ad2d3af4860bb4b861ad0f68b0e315267c36a40576f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:e0e17b700196408888ab48ab7c914db7819ee82f326f2ba2cb6f8fe6d75f4919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262693307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f0adf022ed5d398f0b7f1dbd93f0daf5c2c99f625fc0225a710c59afc1ed1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:31:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:31:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f9c0d1c45afeb74327e597df16894662a900d8c355992eefeeb675d0769066`  
		Last Modified: Tue, 07 Jun 2022 01:53:18 GMT  
		Size: 97.8 MB (97838689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14416f74a08632618c2f5b301b40e1537c737981626b6d5a308c05ac0685cc69`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 275.5 KB (275465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02f37a74d93c667b726c4a1db0b1e11226232ac78f437a285603c07d13d92ca`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53e3e8d33911936f4e2551e3eae9526aa1994e89d0d66c3c0459900bd6d68ba`  
		Last Modified: Tue, 07 Jun 2022 01:53:08 GMT  
		Size: 23.0 MB (23007607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ccc3162be85ff1fa70519bfd257628a728e005b197bf1012a9f11ce2b98cff52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254957822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101c0763c9519ba7c8cae58c6684c706c6ef29b278b56091400ab961143e8f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:06:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:06:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:06:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3035c9ae316d5f3965a292003ea9a80fe4752179a91c4017aa9b0d68e07e6`  
		Last Modified: Tue, 07 Jun 2022 06:24:00 GMT  
		Size: 95.2 MB (95223955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e084c9022832d9836eeda7d8e74c887675c25779e5a393fa13d00d7346d01803`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 275.4 KB (275402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58093b060a5da797812c0b09b2a2da2dbd1417c61297bc1c8d05a88397fb4bf2`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1fdae332ebe53c9728d99ef659e2e4b56a11492df80326566359654277d7ff`  
		Last Modified: Tue, 07 Jun 2022 06:23:50 GMT  
		Size: 22.4 MB (22425056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:4d776d805039fa1a17b7ad2d3af4860bb4b861ad0f68b0e315267c36a40576f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e0e17b700196408888ab48ab7c914db7819ee82f326f2ba2cb6f8fe6d75f4919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262693307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f0adf022ed5d398f0b7f1dbd93f0daf5c2c99f625fc0225a710c59afc1ed1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:31:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:31:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f9c0d1c45afeb74327e597df16894662a900d8c355992eefeeb675d0769066`  
		Last Modified: Tue, 07 Jun 2022 01:53:18 GMT  
		Size: 97.8 MB (97838689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14416f74a08632618c2f5b301b40e1537c737981626b6d5a308c05ac0685cc69`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 275.5 KB (275465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02f37a74d93c667b726c4a1db0b1e11226232ac78f437a285603c07d13d92ca`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53e3e8d33911936f4e2551e3eae9526aa1994e89d0d66c3c0459900bd6d68ba`  
		Last Modified: Tue, 07 Jun 2022 01:53:08 GMT  
		Size: 23.0 MB (23007607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ccc3162be85ff1fa70519bfd257628a728e005b197bf1012a9f11ce2b98cff52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254957822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101c0763c9519ba7c8cae58c6684c706c6ef29b278b56091400ab961143e8f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:06:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:06:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:06:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3035c9ae316d5f3965a292003ea9a80fe4752179a91c4017aa9b0d68e07e6`  
		Last Modified: Tue, 07 Jun 2022 06:24:00 GMT  
		Size: 95.2 MB (95223955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e084c9022832d9836eeda7d8e74c887675c25779e5a393fa13d00d7346d01803`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 275.4 KB (275402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58093b060a5da797812c0b09b2a2da2dbd1417c61297bc1c8d05a88397fb4bf2`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1fdae332ebe53c9728d99ef659e2e4b56a11492df80326566359654277d7ff`  
		Last Modified: Tue, 07 Jun 2022 06:23:50 GMT  
		Size: 22.4 MB (22425056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:522ad56f2df762f5addd19e8c21d984140d9a9a69230c992b569dd8b4708e305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c68a6fe2551f5519fc4e66ca1dcaa6862c1ceda1e510aff1d88eea3e31fe1e93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141569272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbadb9c27f26fbeea8143880dedd4035779e8eb48390578dd5fad296b2ed2ab7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c11a06d3c90baf19298d696dd50b1df397149e2b87b6b865a445e4e862d9b457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137031191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8ae24c7a778204a65c0a9464a5649ed3b7a4f64d944969fe3817e0c4a8ec261`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:522ad56f2df762f5addd19e8c21d984140d9a9a69230c992b569dd8b4708e305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c68a6fe2551f5519fc4e66ca1dcaa6862c1ceda1e510aff1d88eea3e31fe1e93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141569272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbadb9c27f26fbeea8143880dedd4035779e8eb48390578dd5fad296b2ed2ab7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c11a06d3c90baf19298d696dd50b1df397149e2b87b6b865a445e4e862d9b457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137031191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8ae24c7a778204a65c0a9464a5649ed3b7a4f64d944969fe3817e0c4a8ec261`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:4d776d805039fa1a17b7ad2d3af4860bb4b861ad0f68b0e315267c36a40576f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:e0e17b700196408888ab48ab7c914db7819ee82f326f2ba2cb6f8fe6d75f4919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262693307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f0adf022ed5d398f0b7f1dbd93f0daf5c2c99f625fc0225a710c59afc1ed1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 01:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:30:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:30:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:30:14 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:31:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:31:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5978e994b6f023efb223710613e46034904f6dce39ece5e5b8bf07fe938e1`  
		Last Modified: Tue, 07 Jun 2022 01:52:55 GMT  
		Size: 106.1 MB (106124318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff090f1a8ef849bdfa42139c0684e11771a61f5bb61ffba6a2b7c1d2fda9239`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f9c0d1c45afeb74327e597df16894662a900d8c355992eefeeb675d0769066`  
		Last Modified: Tue, 07 Jun 2022 01:53:18 GMT  
		Size: 97.8 MB (97838689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14416f74a08632618c2f5b301b40e1537c737981626b6d5a308c05ac0685cc69`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 275.5 KB (275465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02f37a74d93c667b726c4a1db0b1e11226232ac78f437a285603c07d13d92ca`  
		Last Modified: Tue, 07 Jun 2022 01:53:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53e3e8d33911936f4e2551e3eae9526aa1994e89d0d66c3c0459900bd6d68ba`  
		Last Modified: Tue, 07 Jun 2022 01:53:08 GMT  
		Size: 23.0 MB (23007607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ccc3162be85ff1fa70519bfd257628a728e005b197bf1012a9f11ce2b98cff52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254957822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101c0763c9519ba7c8cae58c6684c706c6ef29b278b56091400ab961143e8f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:05:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:05:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:05:50 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:06:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:06:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:06:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b0c005a3d8c72a2326134dfb835545b11c09e1be826cb6796191a3df42673d`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3035c9ae316d5f3965a292003ea9a80fe4752179a91c4017aa9b0d68e07e6`  
		Last Modified: Tue, 07 Jun 2022 06:24:00 GMT  
		Size: 95.2 MB (95223955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e084c9022832d9836eeda7d8e74c887675c25779e5a393fa13d00d7346d01803`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 275.4 KB (275402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58093b060a5da797812c0b09b2a2da2dbd1417c61297bc1c8d05a88397fb4bf2`  
		Last Modified: Tue, 07 Jun 2022 06:23:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1fdae332ebe53c9728d99ef659e2e4b56a11492df80326566359654277d7ff`  
		Last Modified: Tue, 07 Jun 2022 06:23:50 GMT  
		Size: 22.4 MB (22425056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:220f5c1659c9de350d189df41128cbc7df95d380a813feb319f09859af60d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:51fef39b61f154425a5885bc0a47c218a56b3c433f035a8855f1eb839b91cff4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437402614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11ff77da8460ad832a3be7840a2fdca5baf1185aea1a74138d41cf0efe8c0c05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a26e98e936441e6864a3ca6db9a5eb92d65a3bf52d8f4e07794be2a85ed66bf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385919458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037e0449a6575c838fe3b808a10bbfddcd9fdfe17b9dd2233585c5b294f3b4b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:251824443e3c27f3ccc5424ac09478c73416c179422201b59e58699ca3b44077
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411591074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3774f3961c7bad28536c33f08eba5e39aece6b6ba19fc288c0d8d512bc9cfbc4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:778b7ac964b3b287e4e1774cb04092b792ab1997be19fbd5e88791f1aaa0715a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:69de2426ae25917fd135e13b693c4fdb995ed36691c8670b0fb3dcc403adebbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742717028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b850365c8337f4ca3e77104a142de5d83d2264ef2a7ee4efdfe7a79cd45de127`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:10:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8583c777c2fa9f287b0cfe01be8ccbedd75f900aa5c5134e7f291f2c35e39e1d`  
		Last Modified: Tue, 07 Jun 2022 01:47:07 GMT  
		Size: 305.3 MB (305314414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:43dd4d072ac0a44d6e8eb50e47024d8a439498d5c3f54c1de39567256437d967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (645961486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95099bc8e1c117b21861ff7804ed59d45f73845be87836b04fe287f005e6ab4f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:18:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095115930d6f97863ff374209b9cbefb42259f476e4dafc9e4d8282496ee069a`  
		Last Modified: Tue, 07 Jun 2022 10:38:45 GMT  
		Size: 260.0 MB (260042028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:59fd27f3698d3ad83f834b8e90068125606aea13384d53cdd527c873ad6db0dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (703005048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0beae61f293f59474674e7ab7f8749666423d3d25a9201658d9abd59f2fcd9fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:52:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d94c12966b3c16bedcf101969ae88fa956b72b32ef7e29b343021cc195aa7a`  
		Last Modified: Tue, 07 Jun 2022 06:17:48 GMT  
		Size: 291.4 MB (291413974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:778b7ac964b3b287e4e1774cb04092b792ab1997be19fbd5e88791f1aaa0715a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:69de2426ae25917fd135e13b693c4fdb995ed36691c8670b0fb3dcc403adebbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742717028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b850365c8337f4ca3e77104a142de5d83d2264ef2a7ee4efdfe7a79cd45de127`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:10:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8583c777c2fa9f287b0cfe01be8ccbedd75f900aa5c5134e7f291f2c35e39e1d`  
		Last Modified: Tue, 07 Jun 2022 01:47:07 GMT  
		Size: 305.3 MB (305314414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:43dd4d072ac0a44d6e8eb50e47024d8a439498d5c3f54c1de39567256437d967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (645961486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95099bc8e1c117b21861ff7804ed59d45f73845be87836b04fe287f005e6ab4f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:18:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095115930d6f97863ff374209b9cbefb42259f476e4dafc9e4d8282496ee069a`  
		Last Modified: Tue, 07 Jun 2022 10:38:45 GMT  
		Size: 260.0 MB (260042028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:59fd27f3698d3ad83f834b8e90068125606aea13384d53cdd527c873ad6db0dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (703005048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0beae61f293f59474674e7ab7f8749666423d3d25a9201658d9abd59f2fcd9fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:52:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d94c12966b3c16bedcf101969ae88fa956b72b32ef7e29b343021cc195aa7a`  
		Last Modified: Tue, 07 Jun 2022 06:17:48 GMT  
		Size: 291.4 MB (291413974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:fbedac368afe6a6d379eba815acf34e685529ecd0c1c2ffc1a9ae0fcbb6fb45f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:abf9624b8719c6fd836a5c0803b77b5434fee248a7097dff4753e23ab8a686c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448488064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:522a284b486243807f15fe56d2723bfd034c2b99de4104f787840cc842ff2f1a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:05:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5ffb1f2421f0599334f917713f403ebaea241a7e155f4e6afa5fc492ec43cd`  
		Last Modified: Tue, 07 Jun 2022 01:46:10 GMT  
		Size: 11.1 MB (11085450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:daccd4c05c8dd88ae010fc60bacbf3c37c2bee3930fd13b2324f24d82e7d0965
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396043547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2d6540333253c1f4d762b67772df0f3ac365046370bada96f40baa69cc01be6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d6177d93408b787cd6e05b4693d2262e001e4211f92247d308d6a49805b6bf`  
		Last Modified: Tue, 07 Jun 2022 10:35:52 GMT  
		Size: 10.1 MB (10124089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad01fadf44cb9d22fd3187097376609d1432ffab314aa17f56ebeb98cd0fa349
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422326280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ee6f4bc89ca67e154f17d32c726aa8d469c74cbe7e5e383452ed4271e6f62bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:51:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7836a98ca3a9f6ac7a5369792b042912457e839d10eb1679fb6ce3779dfc56f2`  
		Last Modified: Tue, 07 Jun 2022 06:16:53 GMT  
		Size: 10.7 MB (10735206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:fbedac368afe6a6d379eba815acf34e685529ecd0c1c2ffc1a9ae0fcbb6fb45f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:abf9624b8719c6fd836a5c0803b77b5434fee248a7097dff4753e23ab8a686c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448488064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:522a284b486243807f15fe56d2723bfd034c2b99de4104f787840cc842ff2f1a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:05:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5ffb1f2421f0599334f917713f403ebaea241a7e155f4e6afa5fc492ec43cd`  
		Last Modified: Tue, 07 Jun 2022 01:46:10 GMT  
		Size: 11.1 MB (11085450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:daccd4c05c8dd88ae010fc60bacbf3c37c2bee3930fd13b2324f24d82e7d0965
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396043547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2d6540333253c1f4d762b67772df0f3ac365046370bada96f40baa69cc01be6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d6177d93408b787cd6e05b4693d2262e001e4211f92247d308d6a49805b6bf`  
		Last Modified: Tue, 07 Jun 2022 10:35:52 GMT  
		Size: 10.1 MB (10124089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad01fadf44cb9d22fd3187097376609d1432ffab314aa17f56ebeb98cd0fa349
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422326280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ee6f4bc89ca67e154f17d32c726aa8d469c74cbe7e5e383452ed4271e6f62bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:51:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7836a98ca3a9f6ac7a5369792b042912457e839d10eb1679fb6ce3779dfc56f2`  
		Last Modified: Tue, 07 Jun 2022 06:16:53 GMT  
		Size: 10.7 MB (10735206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:220f5c1659c9de350d189df41128cbc7df95d380a813feb319f09859af60d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:51fef39b61f154425a5885bc0a47c218a56b3c433f035a8855f1eb839b91cff4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437402614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11ff77da8460ad832a3be7840a2fdca5baf1185aea1a74138d41cf0efe8c0c05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:a26e98e936441e6864a3ca6db9a5eb92d65a3bf52d8f4e07794be2a85ed66bf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385919458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037e0449a6575c838fe3b808a10bbfddcd9fdfe17b9dd2233585c5b294f3b4b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:251824443e3c27f3ccc5424ac09478c73416c179422201b59e58699ca3b44077
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411591074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3774f3961c7bad28536c33f08eba5e39aece6b6ba19fc288c0d8d512bc9cfbc4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:220f5c1659c9de350d189df41128cbc7df95d380a813feb319f09859af60d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:51fef39b61f154425a5885bc0a47c218a56b3c433f035a8855f1eb839b91cff4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437402614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11ff77da8460ad832a3be7840a2fdca5baf1185aea1a74138d41cf0efe8c0c05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a26e98e936441e6864a3ca6db9a5eb92d65a3bf52d8f4e07794be2a85ed66bf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385919458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037e0449a6575c838fe3b808a10bbfddcd9fdfe17b9dd2233585c5b294f3b4b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:251824443e3c27f3ccc5424ac09478c73416c179422201b59e58699ca3b44077
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411591074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3774f3961c7bad28536c33f08eba5e39aece6b6ba19fc288c0d8d512bc9cfbc4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:f09675c8557699d34a88fb872ede235023e792d8f28339ad3e539b35efd17f4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:267a888978939abcdbac2d6ba61a46f65eec89b5559bf3771a0fdf70d2acfeeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291880606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be875ec2a73878f10985c35bc23cf15a0e9be149c2f5d4a2098ee00368953ed1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:2e5e7e61d3e85599678a37593d8d28a7f6ae7d2fbbc4205a08b38f4ab2e0434b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266181332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f12379e4d0b5ee9ff52ed6f223b819f8e7db6e58b18ae809377d5932f9da119c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f983915fa697b4b5c4f95aaf5d42d94c7bf4d19c3d322ab5533cf19c92c4ff56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281232232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a8e19427a1a3b0b9921cdff089573ba277646ad583c5a9b90762ea0df2cca8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:f09675c8557699d34a88fb872ede235023e792d8f28339ad3e539b35efd17f4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:267a888978939abcdbac2d6ba61a46f65eec89b5559bf3771a0fdf70d2acfeeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291880606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be875ec2a73878f10985c35bc23cf15a0e9be149c2f5d4a2098ee00368953ed1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:2e5e7e61d3e85599678a37593d8d28a7f6ae7d2fbbc4205a08b38f4ab2e0434b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266181332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f12379e4d0b5ee9ff52ed6f223b819f8e7db6e58b18ae809377d5932f9da119c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f983915fa697b4b5c4f95aaf5d42d94c7bf4d19c3d322ab5533cf19c92c4ff56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281232232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a8e19427a1a3b0b9921cdff089573ba277646ad583c5a9b90762ea0df2cca8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:2016bbb94ff72a95776bda1c0f3c4e6821c8bd57c5e0c6074c84d67efc6a16a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:b6bba9e94e2fc90e9e5346d5b1d5b53f84a3a5aa2537cd39b9d9064f6a8a29ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343020173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6e4c30aaed7605275c4f54e18a856b022baad41e3636a7af7d82f9c59a5330`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:e75166e6b48c9eade1ecae2a4858a50407dc6ae25dcacabcec8bd972b20433e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289170671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89edc59197f1593ae3d5323975da7738dbb11c469245bdab018dc7fc94a18a9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f1b0fb768f15bb0426e4afbf3b98e93667449f8fc90a6e8bbfc33333c732a6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322110264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c9813830776b0f3117791d937028ffd28e03df079c1c24c2d841bea124d3b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:efc4c1e40d16fafbdf5ee1a68a468855b602a89148bd8320419a6d4f0850993f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:75b9e694d8bf831ceeeb7f839faef39718b756fe7fd6b147389b423e81e4deff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834975524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6f96daae1d6f221b7a1e3c317e0e1857ae4406c0cd798c7caea98c423afbcf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b507c79d7107ec363c6307707669011365415eaf3e2b57e092345795a891073`  
		Last Modified: Tue, 07 Jun 2022 01:49:48 GMT  
		Size: 492.0 MB (491955351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:76c31d214cc137ea927ff2063fb650677b35f9425a2bb33a6403f9ea212cac21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726099628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1981d18f271e92ae9f73bd01a9b570ca52867b8c82762839e22e3941de6b65`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:30:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af91be591a3f9fbb984d9d660d7663ce56bf63f386cb93d3a117bc2f204becd`  
		Last Modified: Tue, 07 Jun 2022 10:47:07 GMT  
		Size: 436.9 MB (436928957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abdaf92af631a706682332fa8444b201e5826269a643b8f0c793ae9b3f0271b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.6 MB (784601209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a32e701f93d54e204881bde26d8a04052227b742fa4f4bfcf14734f215f8d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:57:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0301bf829c4c9a911ce71974625824a518faa4957e75948073a0788f5ce1e`  
		Last Modified: Tue, 07 Jun 2022 06:20:26 GMT  
		Size: 462.5 MB (462490945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:439c5b7b7578eaa25b0e863cdc6d60a6774f4a7802bf0dfaf29c9e379321bc87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:252142a6a39f69d3c1d41a05acb3e1321b15cf3a9d3479462d25c073e14cdf17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.4 MB (951370435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e57b97289ee37381b70377b820d6c8b56a5f325f488474f61e4eab5171988d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:31:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:31:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 15:31:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 15:31:04 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 15:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 15:32:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 15:32:08 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:32:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 28 May 2022 15:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:35:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daa03f5fdf981e5e003e8bcdd00a064f8dec5b68d41a8637fa6e6614fb6daa`  
		Last Modified: Sat, 28 May 2022 15:37:19 GMT  
		Size: 10.9 MB (10892084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f843ce8d3b561918a03456323ce94ad1312c2635f4f04d88a0cccf0359be63`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e16ee1496f8cf91f13a0be11f546bcc8a1019871d1ae4a593080f404b5cecdc`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5bca9474dcc4d1c2cb55eb48a9d537e3a19b1977360f0103e67ed68327b2e`  
		Last Modified: Sat, 28 May 2022 15:37:51 GMT  
		Size: 239.2 MB (239165226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7664792e8911a123880c178f4d96e7735082492c404ecedd78d4ebfee2ede`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f466cb7b956c2d5d24b517e11f67106e99b1aadea96679c2c2aa0f36b5948e`  
		Last Modified: Sat, 28 May 2022 15:38:10 GMT  
		Size: 86.6 MB (86570564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328f6c28b3c6930c70d90984ccc80767ee81d5d23ba5124e76bd4e8b7b261a3`  
		Last Modified: Sat, 28 May 2022 15:37:58 GMT  
		Size: 312.9 KB (312930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20422cafa91bad3014676282ceb99ebc8b675eda565d3274d05c57ddc9818011`  
		Last Modified: Sat, 28 May 2022 15:38:08 GMT  
		Size: 76.0 MB (75976311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3465da43dd5d6ee166a07f10d38e641987e9aaed54e08092a562e17edcd6bc8e`  
		Last Modified: Sat, 28 May 2022 15:39:39 GMT  
		Size: 488.0 MB (488010487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6543fa906abf2860d93f71b12a2c292f68afb51d4809a91885c150f91e88b49f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.7 MB (867651907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d73a2e414e817709721b2b7fd0eb3a963f6aad259745f626ff340b5905c9c37e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:31:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:31:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 09:31:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 09:31:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 09:31:50 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 09:31:51 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 09:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 09:33:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 09:33:14 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:33:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 28 May 2022 09:34:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:37:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038e2c6f4de92209486b85dbcdfb0c3794568ec22f4fd2438f984045c9ab600`  
		Last Modified: Sat, 28 May 2022 09:40:41 GMT  
		Size: 10.7 MB (10688315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3e60f35c740bab355e4948391f92c4a13422a4e4c8b87db723eadc9c13293d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986db8ad07690449985043b0f62b086ffb7575f69651d238a6c7914d8964a16a`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687faf58ed162f39e6695b07560ab17b035ad665611906636878c34709ce634`  
		Last Modified: Sat, 28 May 2022 09:41:11 GMT  
		Size: 184.4 MB (184374214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a862c7e717410bf0c285d49d4b7c55f6aa21daeaf531c763e01ba890bd544d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074ba53d7f27638353dab267e782918a7ed0010556584e804cb93de4701ef79b`  
		Last Modified: Sat, 28 May 2022 09:41:29 GMT  
		Size: 84.4 MB (84359217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94008c1f225dc6382751509d1eeffd4225fb329e811d11ff8880fc02717ac95c`  
		Last Modified: Sat, 28 May 2022 09:41:18 GMT  
		Size: 312.9 KB (312868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c12a69a2b5ce14bdc763302315975583e743718ebb8b05509b19227329d001e`  
		Last Modified: Sat, 28 May 2022 09:41:28 GMT  
		Size: 73.9 MB (73865730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ebcb9f37983cff04c112fe18edb638a5a757e65b5ae2984001789d90ff2f16`  
		Last Modified: Sat, 28 May 2022 09:42:54 GMT  
		Size: 464.8 MB (464820140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:efc4c1e40d16fafbdf5ee1a68a468855b602a89148bd8320419a6d4f0850993f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:75b9e694d8bf831ceeeb7f839faef39718b756fe7fd6b147389b423e81e4deff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834975524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6f96daae1d6f221b7a1e3c317e0e1857ae4406c0cd798c7caea98c423afbcf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b507c79d7107ec363c6307707669011365415eaf3e2b57e092345795a891073`  
		Last Modified: Tue, 07 Jun 2022 01:49:48 GMT  
		Size: 492.0 MB (491955351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:76c31d214cc137ea927ff2063fb650677b35f9425a2bb33a6403f9ea212cac21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726099628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1981d18f271e92ae9f73bd01a9b570ca52867b8c82762839e22e3941de6b65`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:30:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af91be591a3f9fbb984d9d660d7663ce56bf63f386cb93d3a117bc2f204becd`  
		Last Modified: Tue, 07 Jun 2022 10:47:07 GMT  
		Size: 436.9 MB (436928957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abdaf92af631a706682332fa8444b201e5826269a643b8f0c793ae9b3f0271b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.6 MB (784601209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a32e701f93d54e204881bde26d8a04052227b742fa4f4bfcf14734f215f8d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:57:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0301bf829c4c9a911ce71974625824a518faa4957e75948073a0788f5ce1e`  
		Last Modified: Tue, 07 Jun 2022 06:20:26 GMT  
		Size: 462.5 MB (462490945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:a61a0c76dd28a6cb404715953f3863bc68080c253e6aaa8f8e8f78fe531ed838
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:532f143a51925de0e4c03c8bd6870373fc35528d4346e82a55de973245eb4342
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358879509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a4d1cb39cc648253519ca70f01dabb2610800f2abaee72fb5cea61c10dbf274`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a683275d5cbaba1dc9e5f38faffcf416f784b536fffb5793b4a6d691baef18de`  
		Last Modified: Tue, 07 Jun 2022 01:48:24 GMT  
		Size: 15.9 MB (15859336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:e899d6df264be7c7f8255c42f13adb0cc568f18531d0947a3d7c0d19a7c6d81c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303235210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00cd235fcd3a2dc7b96329212ed5cf9503ac52e9235946d35900b6c7fc0e803`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c177b6b0d88e56022239c01c0a78bfb4911125de9be40c2057cfbbeb81acb4b2`  
		Last Modified: Tue, 07 Jun 2022 10:42:22 GMT  
		Size: 14.1 MB (14064539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6dc48d76bc35a20213ff111c7d78db95f5e5f356a7d408d36433a6909cdca1b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337558700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c5cbf59e182365eef09ae32d4fe6623e2d8da500193fe96b0e314afd21621c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69fdf059c34f945a771ccbcc56cc3ebf853365c84ba034d76be697f498b2590`  
		Last Modified: Tue, 07 Jun 2022 06:19:09 GMT  
		Size: 15.4 MB (15448436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:629260c4521b3247df0e7a2289c38ec954f8b40bab68d4ed3b4c627b7f43ea9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:50e58478e847d121a86d4816556a11684ecae176b1a9d03d3f92ad96737f2a78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.8 MB (484808290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6936acaef930b0cc0e1f46c0e67a00fd133e4deaf2184fcd0dd9ee0f910e10c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:31:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:31:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 15:31:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 15:31:04 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 15:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 15:32:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 15:32:08 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:32:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 28 May 2022 15:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:33:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daa03f5fdf981e5e003e8bcdd00a064f8dec5b68d41a8637fa6e6614fb6daa`  
		Last Modified: Sat, 28 May 2022 15:37:19 GMT  
		Size: 10.9 MB (10892084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f843ce8d3b561918a03456323ce94ad1312c2635f4f04d88a0cccf0359be63`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e16ee1496f8cf91f13a0be11f546bcc8a1019871d1ae4a593080f404b5cecdc`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5bca9474dcc4d1c2cb55eb48a9d537e3a19b1977360f0103e67ed68327b2e`  
		Last Modified: Sat, 28 May 2022 15:37:51 GMT  
		Size: 239.2 MB (239165226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7664792e8911a123880c178f4d96e7735082492c404ecedd78d4ebfee2ede`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f466cb7b956c2d5d24b517e11f67106e99b1aadea96679c2c2aa0f36b5948e`  
		Last Modified: Sat, 28 May 2022 15:38:10 GMT  
		Size: 86.6 MB (86570564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328f6c28b3c6930c70d90984ccc80767ee81d5d23ba5124e76bd4e8b7b261a3`  
		Last Modified: Sat, 28 May 2022 15:37:58 GMT  
		Size: 312.9 KB (312930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20422cafa91bad3014676282ceb99ebc8b675eda565d3274d05c57ddc9818011`  
		Last Modified: Sat, 28 May 2022 15:38:08 GMT  
		Size: 76.0 MB (75976311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436b651b7982ed73c7a14ccad8204d4be266c53f8caca9a730fdf73481e171c5`  
		Last Modified: Sat, 28 May 2022 15:38:20 GMT  
		Size: 21.4 MB (21448342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4379cffebfd82e9556a65fd6c18e7d3520c3c5da70f942ff407c970d9627e4ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423938507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8239cccc0facfea3f86fa5ae266ff1caa023bc216529a34a3ce81063ebfa0f1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:31:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:31:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 09:31:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 09:31:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 09:31:50 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 09:31:51 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 09:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 09:33:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 09:33:14 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:33:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 28 May 2022 09:34:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:34:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038e2c6f4de92209486b85dbcdfb0c3794568ec22f4fd2438f984045c9ab600`  
		Last Modified: Sat, 28 May 2022 09:40:41 GMT  
		Size: 10.7 MB (10688315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3e60f35c740bab355e4948391f92c4a13422a4e4c8b87db723eadc9c13293d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986db8ad07690449985043b0f62b086ffb7575f69651d238a6c7914d8964a16a`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687faf58ed162f39e6695b07560ab17b035ad665611906636878c34709ce634`  
		Last Modified: Sat, 28 May 2022 09:41:11 GMT  
		Size: 184.4 MB (184374214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a862c7e717410bf0c285d49d4b7c55f6aa21daeaf531c763e01ba890bd544d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074ba53d7f27638353dab267e782918a7ed0010556584e804cb93de4701ef79b`  
		Last Modified: Sat, 28 May 2022 09:41:29 GMT  
		Size: 84.4 MB (84359217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94008c1f225dc6382751509d1eeffd4225fb329e811d11ff8880fc02717ac95c`  
		Last Modified: Sat, 28 May 2022 09:41:18 GMT  
		Size: 312.9 KB (312868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c12a69a2b5ce14bdc763302315975583e743718ebb8b05509b19227329d001e`  
		Last Modified: Sat, 28 May 2022 09:41:28 GMT  
		Size: 73.9 MB (73865730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec076d605ab54bd35291bb3ee6fea64c2896123a8210550888042fb3e0b81c84`  
		Last Modified: Sat, 28 May 2022 09:41:40 GMT  
		Size: 21.1 MB (21106740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:a61a0c76dd28a6cb404715953f3863bc68080c253e6aaa8f8e8f78fe531ed838
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:532f143a51925de0e4c03c8bd6870373fc35528d4346e82a55de973245eb4342
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358879509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a4d1cb39cc648253519ca70f01dabb2610800f2abaee72fb5cea61c10dbf274`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a683275d5cbaba1dc9e5f38faffcf416f784b536fffb5793b4a6d691baef18de`  
		Last Modified: Tue, 07 Jun 2022 01:48:24 GMT  
		Size: 15.9 MB (15859336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:e899d6df264be7c7f8255c42f13adb0cc568f18531d0947a3d7c0d19a7c6d81c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303235210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00cd235fcd3a2dc7b96329212ed5cf9503ac52e9235946d35900b6c7fc0e803`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c177b6b0d88e56022239c01c0a78bfb4911125de9be40c2057cfbbeb81acb4b2`  
		Last Modified: Tue, 07 Jun 2022 10:42:22 GMT  
		Size: 14.1 MB (14064539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6dc48d76bc35a20213ff111c7d78db95f5e5f356a7d408d36433a6909cdca1b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337558700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c5cbf59e182365eef09ae32d4fe6623e2d8da500193fe96b0e314afd21621c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69fdf059c34f945a771ccbcc56cc3ebf853365c84ba034d76be697f498b2590`  
		Last Modified: Tue, 07 Jun 2022 06:19:09 GMT  
		Size: 15.4 MB (15448436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:2016bbb94ff72a95776bda1c0f3c4e6821c8bd57c5e0c6074c84d67efc6a16a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b6bba9e94e2fc90e9e5346d5b1d5b53f84a3a5aa2537cd39b9d9064f6a8a29ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343020173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6e4c30aaed7605275c4f54e18a856b022baad41e3636a7af7d82f9c59a5330`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:e75166e6b48c9eade1ecae2a4858a50407dc6ae25dcacabcec8bd972b20433e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289170671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89edc59197f1593ae3d5323975da7738dbb11c469245bdab018dc7fc94a18a9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f1b0fb768f15bb0426e4afbf3b98e93667449f8fc90a6e8bbfc33333c732a6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322110264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c9813830776b0f3117791d937028ffd28e03df079c1c24c2d841bea124d3b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:f4e3ce40e01c0012617d79b685e8f28dee9c6316cfe61f045cc67d4a544dc415
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:0b37a6613771055e90bb0887ba011f6ff7c45b76a2e5b9893c395b901d56e118
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463359948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1787fc9fbba7cce41d505c70929c0e44fc93a728c92d389afb7b6e6645b7585e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:31:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:31:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 15:31:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 15:31:04 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 15:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 15:32:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 15:32:08 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:32:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 28 May 2022 15:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daa03f5fdf981e5e003e8bcdd00a064f8dec5b68d41a8637fa6e6614fb6daa`  
		Last Modified: Sat, 28 May 2022 15:37:19 GMT  
		Size: 10.9 MB (10892084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f843ce8d3b561918a03456323ce94ad1312c2635f4f04d88a0cccf0359be63`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e16ee1496f8cf91f13a0be11f546bcc8a1019871d1ae4a593080f404b5cecdc`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5bca9474dcc4d1c2cb55eb48a9d537e3a19b1977360f0103e67ed68327b2e`  
		Last Modified: Sat, 28 May 2022 15:37:51 GMT  
		Size: 239.2 MB (239165226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7664792e8911a123880c178f4d96e7735082492c404ecedd78d4ebfee2ede`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f466cb7b956c2d5d24b517e11f67106e99b1aadea96679c2c2aa0f36b5948e`  
		Last Modified: Sat, 28 May 2022 15:38:10 GMT  
		Size: 86.6 MB (86570564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328f6c28b3c6930c70d90984ccc80767ee81d5d23ba5124e76bd4e8b7b261a3`  
		Last Modified: Sat, 28 May 2022 15:37:58 GMT  
		Size: 312.9 KB (312930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20422cafa91bad3014676282ceb99ebc8b675eda565d3274d05c57ddc9818011`  
		Last Modified: Sat, 28 May 2022 15:38:08 GMT  
		Size: 76.0 MB (75976311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fd0b876aa029ea6226945fbee4a8fadc09d35263efa75fecf79812c138965a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.8 MB (402831767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22148c2b16ee84c7ed30829b5c37431758d362281b397075b76c6159a23787b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:31:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:31:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 09:31:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 09:31:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 09:31:50 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 09:31:51 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 09:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 09:33:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 09:33:14 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:33:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 28 May 2022 09:34:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038e2c6f4de92209486b85dbcdfb0c3794568ec22f4fd2438f984045c9ab600`  
		Last Modified: Sat, 28 May 2022 09:40:41 GMT  
		Size: 10.7 MB (10688315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3e60f35c740bab355e4948391f92c4a13422a4e4c8b87db723eadc9c13293d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986db8ad07690449985043b0f62b086ffb7575f69651d238a6c7914d8964a16a`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687faf58ed162f39e6695b07560ab17b035ad665611906636878c34709ce634`  
		Last Modified: Sat, 28 May 2022 09:41:11 GMT  
		Size: 184.4 MB (184374214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a862c7e717410bf0c285d49d4b7c55f6aa21daeaf531c763e01ba890bd544d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074ba53d7f27638353dab267e782918a7ed0010556584e804cb93de4701ef79b`  
		Last Modified: Sat, 28 May 2022 09:41:29 GMT  
		Size: 84.4 MB (84359217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94008c1f225dc6382751509d1eeffd4225fb329e811d11ff8880fc02717ac95c`  
		Last Modified: Sat, 28 May 2022 09:41:18 GMT  
		Size: 312.9 KB (312868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c12a69a2b5ce14bdc763302315975583e743718ebb8b05509b19227329d001e`  
		Last Modified: Sat, 28 May 2022 09:41:28 GMT  
		Size: 73.9 MB (73865730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:2016bbb94ff72a95776bda1c0f3c4e6821c8bd57c5e0c6074c84d67efc6a16a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:b6bba9e94e2fc90e9e5346d5b1d5b53f84a3a5aa2537cd39b9d9064f6a8a29ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343020173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6e4c30aaed7605275c4f54e18a856b022baad41e3636a7af7d82f9c59a5330`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:e75166e6b48c9eade1ecae2a4858a50407dc6ae25dcacabcec8bd972b20433e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289170671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89edc59197f1593ae3d5323975da7738dbb11c469245bdab018dc7fc94a18a9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f1b0fb768f15bb0426e4afbf3b98e93667449f8fc90a6e8bbfc33333c732a6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322110264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c9813830776b0f3117791d937028ffd28e03df079c1c24c2d841bea124d3b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:ffabb5f204a6915a655db1f814a3187a42158f17340fb1b2d656bcf829f9651d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5c9098c9c040336f8d3c9f5cf8b3605d45ef385acac7d2a2a34a0f0db74adceb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212163558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ed23f6e8227392712cbd506b39edf2ba24768a059cc8c14cd19d062a7a069d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:142a88b56842c0388ab1312095b5ddda51ad21b0108fa4eb769b4845e843bcfd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187869062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a84dbac57278e679c7ddd3ef4efd476f35999017219698bb27623de8d8354e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:682f7c3f519d3703f61ccda15a7122e3a6cb4f76bd6dfd1576745c4cf469074d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205047523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d13ae14e7cf6620f1d62f4d952df1b69ecf5fc476b9c3e28a1a5e8d07660b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:58d005ec9465e0fe95b72a59234905c0f4e4ecfd4216910e317af67abcb60252
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:03e17e6317e4e65d58883d37ba8b05a6bb805786480e4c0862d35af530ba8a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300500143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf67f584ec11e38d39fcb8aa4cc831f033362886f1e04c65c08fe1a638e0c672`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:31:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:31:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 15:31:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 15:31:04 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 15:31:04 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 15:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:32:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 15:32:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 15:32:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daa03f5fdf981e5e003e8bcdd00a064f8dec5b68d41a8637fa6e6614fb6daa`  
		Last Modified: Sat, 28 May 2022 15:37:19 GMT  
		Size: 10.9 MB (10892084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f843ce8d3b561918a03456323ce94ad1312c2635f4f04d88a0cccf0359be63`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e16ee1496f8cf91f13a0be11f546bcc8a1019871d1ae4a593080f404b5cecdc`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5bca9474dcc4d1c2cb55eb48a9d537e3a19b1977360f0103e67ed68327b2e`  
		Last Modified: Sat, 28 May 2022 15:37:51 GMT  
		Size: 239.2 MB (239165226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7664792e8911a123880c178f4d96e7735082492c404ecedd78d4ebfee2ede`  
		Last Modified: Sat, 28 May 2022 15:37:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fa6f900f8bc4964429c7cec97fc45e7755e94ab2b16b7e4dc1ade8d90af5ebd0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244293952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09146ff9c87a825048dba6a2047746045307900a5641c45537539fc17dc3280a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:31:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:31:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 May 2022 09:31:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 May 2022 09:31:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 09:31:50 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 May 2022 09:31:51 GMT
ENV ROS_DISTRO=noetic
# Sat, 28 May 2022 09:33:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:33:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 May 2022 09:33:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 May 2022 09:33:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038e2c6f4de92209486b85dbcdfb0c3794568ec22f4fd2438f984045c9ab600`  
		Last Modified: Sat, 28 May 2022 09:40:41 GMT  
		Size: 10.7 MB (10688315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3e60f35c740bab355e4948391f92c4a13422a4e4c8b87db723eadc9c13293d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986db8ad07690449985043b0f62b086ffb7575f69651d238a6c7914d8964a16a`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687faf58ed162f39e6695b07560ab17b035ad665611906636878c34709ce634`  
		Last Modified: Sat, 28 May 2022 09:41:11 GMT  
		Size: 184.4 MB (184374214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a862c7e717410bf0c285d49d4b7c55f6aa21daeaf531c763e01ba890bd544d`  
		Last Modified: Sat, 28 May 2022 09:40:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:ffabb5f204a6915a655db1f814a3187a42158f17340fb1b2d656bcf829f9651d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:5c9098c9c040336f8d3c9f5cf8b3605d45ef385acac7d2a2a34a0f0db74adceb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212163558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ed23f6e8227392712cbd506b39edf2ba24768a059cc8c14cd19d062a7a069d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:142a88b56842c0388ab1312095b5ddda51ad21b0108fa4eb769b4845e843bcfd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187869062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a84dbac57278e679c7ddd3ef4efd476f35999017219698bb27623de8d8354e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:682f7c3f519d3703f61ccda15a7122e3a6cb4f76bd6dfd1576745c4cf469074d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205047523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d13ae14e7cf6620f1d62f4d952df1b69ecf5fc476b9c3e28a1a5e8d07660b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:6eebba1d7d8127f90cd790964c23521597aba363fa60ec1a387895b1274c8484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:da1a2d2e9e41bd9c29cb3c99a8cb4b45f8d8c87fbab20c8f3399819bebb74de8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262719439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436e82c5b0bca3bd441eaded5e62eefc4c3b7bfa6903d1a814e70b9192e560ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:41:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:41:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e141275ac844961d5e6aae4adaff24bbc71e569676a50e4ceb83aac78b808c03`  
		Last Modified: Tue, 07 Jun 2022 01:56:14 GMT  
		Size: 97.8 MB (97838742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecab1f16ec251a3dfbd7c86db15d68f7937ac612f6b6342c89b6f7272eeb318`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 273.2 KB (273161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e01aa968f971f9b30c74f1b45be67addb7b3ac071b1d2879a5f99184f6bd40c`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf2ef0c2f0d6cdbddea8135625ff2a75b8f0358d46a81e65d0e8622c5bf671`  
		Last Modified: Tue, 07 Jun 2022 01:56:04 GMT  
		Size: 23.0 MB (23028911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41b8bc478d097ea077e2d01bf81624f9836ad30ba3ae9a2bef03c148369a1038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254977578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8807bdd5c76dea927a5e6a26a7ad603b8cc5fac7625f14815dfda17213ce482b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:10:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:11:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9904a4fe7a75f1eed88c54411c41df21cea85b5e1eee36bfc1426a6c355b152`  
		Last Modified: Tue, 07 Jun 2022 06:26:45 GMT  
		Size: 95.2 MB (95223816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d35cdddc2acfbc5c458c06a2df30fb69d28a1fe576252273c8f5d734335eb83`  
		Last Modified: Tue, 07 Jun 2022 06:26:32 GMT  
		Size: 273.1 KB (273097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c7be9982d5ae74dffb3e90ca2f2b866364281b12e84fd5373efc8e07565cd`  
		Last Modified: Tue, 07 Jun 2022 06:26:31 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d873c09a237a9c1df0a3031bef8211427e58da4c8fb2f6a0a5b06b8d9f27353`  
		Last Modified: Tue, 07 Jun 2022 06:26:35 GMT  
		Size: 22.4 MB (22444556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:72279dcab238e47fb7a72bb8873853a8ea6478c585d1e6a798b85831c69bb8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:ced8864c2d75e792a99477c9c834b3bf89d3b790844e2c940ce853d6d3ebc258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1089346218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96597a8b0aff9e01b9210fe01ccd5c9c752b1051f94c8245fc9be5832c936940`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:41:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:41:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e141275ac844961d5e6aae4adaff24bbc71e569676a50e4ceb83aac78b808c03`  
		Last Modified: Tue, 07 Jun 2022 01:56:14 GMT  
		Size: 97.8 MB (97838742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecab1f16ec251a3dfbd7c86db15d68f7937ac612f6b6342c89b6f7272eeb318`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 273.2 KB (273161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e01aa968f971f9b30c74f1b45be67addb7b3ac071b1d2879a5f99184f6bd40c`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf2ef0c2f0d6cdbddea8135625ff2a75b8f0358d46a81e65d0e8622c5bf671`  
		Last Modified: Tue, 07 Jun 2022 01:56:04 GMT  
		Size: 23.0 MB (23028911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ebfd09fa4334182f0f38bc21a84ec55fee678b3043115137a7d49905e9d48`  
		Last Modified: Tue, 07 Jun 2022 01:58:06 GMT  
		Size: 826.6 MB (826626779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:465d6d4d7feef1d3b6720d3dca739f2a3aa93b4a51b5b13b6fd49db6eec8bcb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034071472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a17d9b9b0a9fbf9991e2a3bc2af25978d0ba195e794f2c294eb3a7ea290e1f5c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:10:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:11:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9904a4fe7a75f1eed88c54411c41df21cea85b5e1eee36bfc1426a6c355b152`  
		Last Modified: Tue, 07 Jun 2022 06:26:45 GMT  
		Size: 95.2 MB (95223816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d35cdddc2acfbc5c458c06a2df30fb69d28a1fe576252273c8f5d734335eb83`  
		Last Modified: Tue, 07 Jun 2022 06:26:32 GMT  
		Size: 273.1 KB (273097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c7be9982d5ae74dffb3e90ca2f2b866364281b12e84fd5373efc8e07565cd`  
		Last Modified: Tue, 07 Jun 2022 06:26:31 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d873c09a237a9c1df0a3031bef8211427e58da4c8fb2f6a0a5b06b8d9f27353`  
		Last Modified: Tue, 07 Jun 2022 06:26:35 GMT  
		Size: 22.4 MB (22444556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03371cd79205b6bd19d255dca67afd2e09d45aba4666e67d1b82ba51ded55a2b`  
		Last Modified: Tue, 07 Jun 2022 06:28:33 GMT  
		Size: 779.1 MB (779093894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:72279dcab238e47fb7a72bb8873853a8ea6478c585d1e6a798b85831c69bb8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:ced8864c2d75e792a99477c9c834b3bf89d3b790844e2c940ce853d6d3ebc258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1089346218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96597a8b0aff9e01b9210fe01ccd5c9c752b1051f94c8245fc9be5832c936940`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:41:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:41:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e141275ac844961d5e6aae4adaff24bbc71e569676a50e4ceb83aac78b808c03`  
		Last Modified: Tue, 07 Jun 2022 01:56:14 GMT  
		Size: 97.8 MB (97838742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecab1f16ec251a3dfbd7c86db15d68f7937ac612f6b6342c89b6f7272eeb318`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 273.2 KB (273161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e01aa968f971f9b30c74f1b45be67addb7b3ac071b1d2879a5f99184f6bd40c`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf2ef0c2f0d6cdbddea8135625ff2a75b8f0358d46a81e65d0e8622c5bf671`  
		Last Modified: Tue, 07 Jun 2022 01:56:04 GMT  
		Size: 23.0 MB (23028911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ebfd09fa4334182f0f38bc21a84ec55fee678b3043115137a7d49905e9d48`  
		Last Modified: Tue, 07 Jun 2022 01:58:06 GMT  
		Size: 826.6 MB (826626779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:465d6d4d7feef1d3b6720d3dca739f2a3aa93b4a51b5b13b6fd49db6eec8bcb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034071472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a17d9b9b0a9fbf9991e2a3bc2af25978d0ba195e794f2c294eb3a7ea290e1f5c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:10:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:11:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9904a4fe7a75f1eed88c54411c41df21cea85b5e1eee36bfc1426a6c355b152`  
		Last Modified: Tue, 07 Jun 2022 06:26:45 GMT  
		Size: 95.2 MB (95223816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d35cdddc2acfbc5c458c06a2df30fb69d28a1fe576252273c8f5d734335eb83`  
		Last Modified: Tue, 07 Jun 2022 06:26:32 GMT  
		Size: 273.1 KB (273097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c7be9982d5ae74dffb3e90ca2f2b866364281b12e84fd5373efc8e07565cd`  
		Last Modified: Tue, 07 Jun 2022 06:26:31 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d873c09a237a9c1df0a3031bef8211427e58da4c8fb2f6a0a5b06b8d9f27353`  
		Last Modified: Tue, 07 Jun 2022 06:26:35 GMT  
		Size: 22.4 MB (22444556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03371cd79205b6bd19d255dca67afd2e09d45aba4666e67d1b82ba51ded55a2b`  
		Last Modified: Tue, 07 Jun 2022 06:28:33 GMT  
		Size: 779.1 MB (779093894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:6eebba1d7d8127f90cd790964c23521597aba363fa60ec1a387895b1274c8484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:da1a2d2e9e41bd9c29cb3c99a8cb4b45f8d8c87fbab20c8f3399819bebb74de8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262719439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436e82c5b0bca3bd441eaded5e62eefc4c3b7bfa6903d1a814e70b9192e560ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:41:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:41:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e141275ac844961d5e6aae4adaff24bbc71e569676a50e4ceb83aac78b808c03`  
		Last Modified: Tue, 07 Jun 2022 01:56:14 GMT  
		Size: 97.8 MB (97838742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecab1f16ec251a3dfbd7c86db15d68f7937ac612f6b6342c89b6f7272eeb318`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 273.2 KB (273161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e01aa968f971f9b30c74f1b45be67addb7b3ac071b1d2879a5f99184f6bd40c`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf2ef0c2f0d6cdbddea8135625ff2a75b8f0358d46a81e65d0e8622c5bf671`  
		Last Modified: Tue, 07 Jun 2022 01:56:04 GMT  
		Size: 23.0 MB (23028911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41b8bc478d097ea077e2d01bf81624f9836ad30ba3ae9a2bef03c148369a1038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254977578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8807bdd5c76dea927a5e6a26a7ad603b8cc5fac7625f14815dfda17213ce482b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:10:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:11:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9904a4fe7a75f1eed88c54411c41df21cea85b5e1eee36bfc1426a6c355b152`  
		Last Modified: Tue, 07 Jun 2022 06:26:45 GMT  
		Size: 95.2 MB (95223816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d35cdddc2acfbc5c458c06a2df30fb69d28a1fe576252273c8f5d734335eb83`  
		Last Modified: Tue, 07 Jun 2022 06:26:32 GMT  
		Size: 273.1 KB (273097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c7be9982d5ae74dffb3e90ca2f2b866364281b12e84fd5373efc8e07565cd`  
		Last Modified: Tue, 07 Jun 2022 06:26:31 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d873c09a237a9c1df0a3031bef8211427e58da4c8fb2f6a0a5b06b8d9f27353`  
		Last Modified: Tue, 07 Jun 2022 06:26:35 GMT  
		Size: 22.4 MB (22444556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:6eebba1d7d8127f90cd790964c23521597aba363fa60ec1a387895b1274c8484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:da1a2d2e9e41bd9c29cb3c99a8cb4b45f8d8c87fbab20c8f3399819bebb74de8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262719439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436e82c5b0bca3bd441eaded5e62eefc4c3b7bfa6903d1a814e70b9192e560ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:41:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:41:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 01:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e141275ac844961d5e6aae4adaff24bbc71e569676a50e4ceb83aac78b808c03`  
		Last Modified: Tue, 07 Jun 2022 01:56:14 GMT  
		Size: 97.8 MB (97838742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecab1f16ec251a3dfbd7c86db15d68f7937ac612f6b6342c89b6f7272eeb318`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 273.2 KB (273161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e01aa968f971f9b30c74f1b45be67addb7b3ac071b1d2879a5f99184f6bd40c`  
		Last Modified: Tue, 07 Jun 2022 01:56:00 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cf2ef0c2f0d6cdbddea8135625ff2a75b8f0358d46a81e65d0e8622c5bf671`  
		Last Modified: Tue, 07 Jun 2022 01:56:04 GMT  
		Size: 23.0 MB (23028911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41b8bc478d097ea077e2d01bf81624f9836ad30ba3ae9a2bef03c148369a1038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254977578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8807bdd5c76dea927a5e6a26a7ad603b8cc5fac7625f14815dfda17213ce482b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:10:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:11:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jun 2022 06:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9904a4fe7a75f1eed88c54411c41df21cea85b5e1eee36bfc1426a6c355b152`  
		Last Modified: Tue, 07 Jun 2022 06:26:45 GMT  
		Size: 95.2 MB (95223816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d35cdddc2acfbc5c458c06a2df30fb69d28a1fe576252273c8f5d734335eb83`  
		Last Modified: Tue, 07 Jun 2022 06:26:32 GMT  
		Size: 273.1 KB (273097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c7be9982d5ae74dffb3e90ca2f2b866364281b12e84fd5373efc8e07565cd`  
		Last Modified: Tue, 07 Jun 2022 06:26:31 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d873c09a237a9c1df0a3031bef8211427e58da4c8fb2f6a0a5b06b8d9f27353`  
		Last Modified: Tue, 07 Jun 2022 06:26:35 GMT  
		Size: 22.4 MB (22444556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:31060ab128c31452f13050c1f33be98d4cf55ec5e82b3f30ba412aa591d4b1f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:8649d3ff11624e61eb7c7010fc0f186f21cd8e4a0ad1d2c27c9a39dc8a59987d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141576353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0f3d817c57e9ce4d4ed7eb90d07248e52f585c283694c87e3bbf4617cf8266`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:584b4a954ab5c2f9e93db6ab4203b3aabd63972588b1a7390d05a5e77146e030
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137033918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a32cb70f30887f91017990a2de90e207ce6885b11168273eee70d0b3d4ed9a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:31060ab128c31452f13050c1f33be98d4cf55ec5e82b3f30ba412aa591d4b1f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:8649d3ff11624e61eb7c7010fc0f186f21cd8e4a0ad1d2c27c9a39dc8a59987d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141576353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0f3d817c57e9ce4d4ed7eb90d07248e52f585c283694c87e3bbf4617cf8266`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:28:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:28:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 01:28:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:28:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:40:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 01:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:41:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 01:41:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:41:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1d4bf62a3722d7122bc1b8ee8ad3051fcaf598ca72ad725fea76cb53f6b3c`  
		Last Modified: Tue, 07 Jun 2022 01:52:41 GMT  
		Size: 1.2 MB (1191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5c906965a7cb2488a6e23da68abe175ee9acffbe27e61b1152cfff4fbf840b`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 3.8 MB (3827182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1af53ce2d5965bf4c8489cf5459894d2e6c3f6b00538c076d38e41668d6cf`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8d3945eb76a1a2076630ee2752a89342d614a9298134e198075975ec08400d`  
		Last Modified: Tue, 07 Jun 2022 01:52:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c71936f086360e13475372b678edf9e90dda0249fc0cb007070b136f0b431`  
		Last Modified: Tue, 07 Jun 2022 01:55:42 GMT  
		Size: 106.1 MB (106131399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba72d83ed0d2e6bbd2f45b43761d9699bdc1bdeecc565de30d7c4c75696f0b5`  
		Last Modified: Tue, 07 Jun 2022 01:55:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:584b4a954ab5c2f9e93db6ab4203b3aabd63972588b1a7390d05a5e77146e030
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137033918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a32cb70f30887f91017990a2de90e207ce6885b11168273eee70d0b3d4ed9a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:09:33 GMT
ENV ROS_DISTRO=rolling
# Tue, 07 Jun 2022 06:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:10:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jun 2022 06:10:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 06:10:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afae557291fb262be019f4a220aeb20ea7c6b1474c968d4bb9d8ba63e5295e39`  
		Last Modified: Tue, 07 Jun 2022 06:26:21 GMT  
		Size: 103.9 MB (103865174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aab77c96357ad802c699db548bd10726e6a4ac599df8ef215e6ddfe925444b`  
		Last Modified: Tue, 07 Jun 2022 06:26:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
