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
$ docker pull ros@sha256:f7299f4eb820c59adaeb9c16af428ac3e0aab0ff38735cd453145c4c4cbf79d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:18e9dbacc08da9636fe5c515d7303715d0e87d15a53879ccab9d979087ba9a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251846325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c645eb93f5e52feb828db0e9fa5f313ca3c35a01dd8ebff251680537d6ad3403`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2f629aab5a540a63cdbc508dda1e8c60d49c4eeb5d94de9f4998b41b93fc8da5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227242523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5a452b850177955c2793a3f03ec97ac920e348c663671a2f538cafff7011118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:f7299f4eb820c59adaeb9c16af428ac3e0aab0ff38735cd453145c4c4cbf79d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:18e9dbacc08da9636fe5c515d7303715d0e87d15a53879ccab9d979087ba9a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251846325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c645eb93f5e52feb828db0e9fa5f313ca3c35a01dd8ebff251680537d6ad3403`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2f629aab5a540a63cdbc508dda1e8c60d49c4eeb5d94de9f4998b41b93fc8da5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227242523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5a452b850177955c2793a3f03ec97ac920e348c663671a2f538cafff7011118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:f7299f4eb820c59adaeb9c16af428ac3e0aab0ff38735cd453145c4c4cbf79d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:18e9dbacc08da9636fe5c515d7303715d0e87d15a53879ccab9d979087ba9a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251846325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c645eb93f5e52feb828db0e9fa5f313ca3c35a01dd8ebff251680537d6ad3403`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2f629aab5a540a63cdbc508dda1e8c60d49c4eeb5d94de9f4998b41b93fc8da5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227242523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5a452b850177955c2793a3f03ec97ac920e348c663671a2f538cafff7011118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:112e28d725d9a251cde081edc16831b4ab005dd16d874575996e37c18562c3b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:1323f3efb34e39faf1164fc87cfe0465a3e8b2099bef1d297ed3d66afe7e1d81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155380717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ad8dd08c800843587e3d2836c25d19c199bc3a90245ff114b31365247ddf3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bf17798fa54f2723ff2dc07ec9b6c8bb443327a2d688e3f2d4cd15d42a15f55e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137941706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682295c93e67b4ea3975461860a919fcda01b098e8eedb420165db1ed6678ebc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:112e28d725d9a251cde081edc16831b4ab005dd16d874575996e37c18562c3b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:1323f3efb34e39faf1164fc87cfe0465a3e8b2099bef1d297ed3d66afe7e1d81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155380717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ad8dd08c800843587e3d2836c25d19c199bc3a90245ff114b31365247ddf3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bf17798fa54f2723ff2dc07ec9b6c8bb443327a2d688e3f2d4cd15d42a15f55e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137941706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682295c93e67b4ea3975461860a919fcda01b098e8eedb420165db1ed6678ebc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:6e5504e7240a4719023081dec783080a8f558ce1aa39f35fb9576ec0783202cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:f6f5c0a0e4853ebcb1d0c793d490da59bd2d64e6a5f872210082b42730db3f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.7 MB (349716175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0977093e1753c1bf7fb7338dbbbce5e7fe7a1baee3a2b24ab01af46d236e91f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:39:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:39:14 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 03:39:14 GMT
ENV ROS2_DISTRO=foxy
# Fri, 22 Apr 2022 03:39:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b5f330b17bff3b79078ad4a779b74b71742d53f1bd9cb4bf256ab89fe6d3e`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308cbc359a788776e176402454db5b48e363e38d8fbbcb052472da3aac8d9206`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea5382ebe2ec51b07e3e93c6d68facc813a488754b27f195e36931889ddf7`  
		Last Modified: Fri, 22 Apr 2022 03:53:36 GMT  
		Size: 76.3 MB (76324782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c672e567bbdbc2ec09e3bf6b2f3e362e0a23eb023827223ce11a4463938b298`  
		Last Modified: Fri, 22 Apr 2022 03:53:26 GMT  
		Size: 21.5 MB (21544441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1febcc87ce4e65c78a1ec45e36df3fa2099f9b70f8e76560cb9db11e7c769834`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:695bd97e5fb12c16202e36da61191fe713ff2147ec22b12f0f31f1247b205ee2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317361780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033c4c76d50f082c86ab16441b0145598eddcb5e4d0b9ae80b8f4efb79750e58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:10:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:10:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:10:29 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 04:10:31 GMT
ENV ROS2_DISTRO=foxy
# Fri, 22 Apr 2022 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:11:25 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d1a8875302bc9d8a9c3e4061ee2ab7fbcaf59d55558650697341e3a352bcd`  
		Last Modified: Fri, 22 Apr 2022 04:25:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b72035e559f367a7be9a0d6dff792faa3991f692cbba74968ea9e80a0e626d`  
		Last Modified: Fri, 22 Apr 2022 04:25:41 GMT  
		Size: 76.2 MB (76154125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435a6ce1a0bfebd525543e64b85ef20039c3967cc6ca6e9bca0d351a2288854e`  
		Last Modified: Fri, 22 Apr 2022 04:25:29 GMT  
		Size: 14.0 MB (13964662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5aff43097bc70c117dae8f182a5e6c6cfbf1a439b2d8baef3e3349936ffd4f`  
		Last Modified: Fri, 22 Apr 2022 04:25:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:6e5504e7240a4719023081dec783080a8f558ce1aa39f35fb9576ec0783202cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:f6f5c0a0e4853ebcb1d0c793d490da59bd2d64e6a5f872210082b42730db3f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.7 MB (349716175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0977093e1753c1bf7fb7338dbbbce5e7fe7a1baee3a2b24ab01af46d236e91f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:39:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:39:14 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 03:39:14 GMT
ENV ROS2_DISTRO=foxy
# Fri, 22 Apr 2022 03:39:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b5f330b17bff3b79078ad4a779b74b71742d53f1bd9cb4bf256ab89fe6d3e`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308cbc359a788776e176402454db5b48e363e38d8fbbcb052472da3aac8d9206`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea5382ebe2ec51b07e3e93c6d68facc813a488754b27f195e36931889ddf7`  
		Last Modified: Fri, 22 Apr 2022 03:53:36 GMT  
		Size: 76.3 MB (76324782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c672e567bbdbc2ec09e3bf6b2f3e362e0a23eb023827223ce11a4463938b298`  
		Last Modified: Fri, 22 Apr 2022 03:53:26 GMT  
		Size: 21.5 MB (21544441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1febcc87ce4e65c78a1ec45e36df3fa2099f9b70f8e76560cb9db11e7c769834`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:695bd97e5fb12c16202e36da61191fe713ff2147ec22b12f0f31f1247b205ee2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317361780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033c4c76d50f082c86ab16441b0145598eddcb5e4d0b9ae80b8f4efb79750e58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:10:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:10:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:10:29 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 04:10:31 GMT
ENV ROS2_DISTRO=foxy
# Fri, 22 Apr 2022 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:11:25 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d1a8875302bc9d8a9c3e4061ee2ab7fbcaf59d55558650697341e3a352bcd`  
		Last Modified: Fri, 22 Apr 2022 04:25:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b72035e559f367a7be9a0d6dff792faa3991f692cbba74968ea9e80a0e626d`  
		Last Modified: Fri, 22 Apr 2022 04:25:41 GMT  
		Size: 76.2 MB (76154125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435a6ce1a0bfebd525543e64b85ef20039c3967cc6ca6e9bca0d351a2288854e`  
		Last Modified: Fri, 22 Apr 2022 04:25:29 GMT  
		Size: 14.0 MB (13964662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5aff43097bc70c117dae8f182a5e6c6cfbf1a439b2d8baef3e3349936ffd4f`  
		Last Modified: Fri, 22 Apr 2022 04:25:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:05ff07940a5ed666b30f0e9cb3e5989e3d0af92393950351c418c5ccc8703137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:57982240c0b1d9639b5d4017bd39fd04ffb6e1947f059b9bb2c46320879db806
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235830367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf1eab5ff47ea02c884e6f99e01b82106247185704ba244505d93fa6ec51b75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:41:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:41:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:41:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d81b4f14257aafe9c36754217f7b33e5594f7991bdc5fed442f3e351818ca6`  
		Last Modified: Fri, 22 Apr 2022 03:54:26 GMT  
		Size: 74.5 MB (74494199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86ee117572ea9ab37045a8143bd74f2c6fc866407f2c1b855fef3c348bec9f6`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 262.2 KB (262250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc056e4b5fb80b3e3a36e14d46061812f16e11166015dfbf5c8e9f911b4bc5e0`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a725f33deb8c6696fb2fe8f21c3fe0f20e6598f23354c10b3d1953701fe651`  
		Last Modified: Fri, 22 Apr 2022 03:54:18 GMT  
		Size: 22.1 MB (22113636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:226fa8b063571c73b4edede044f3a5c5dd59c24dcd749be5af219ae29ab60229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224032026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea80bb6394b0a866f1da8a2d6bbf18c448a676b6ac18e4c23c17c3926c256d41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:14:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04358f3e939d7f9f6a53c0ecd2c599e6321d2b4b0c0e9978c2dc6f05632e9711`  
		Last Modified: Fri, 22 Apr 2022 04:26:32 GMT  
		Size: 68.6 MB (68617910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cf32eefb7bf397b5f31ea8c519a7b26f428c65adf974fcbef5723a3b4d940`  
		Last Modified: Fri, 22 Apr 2022 04:26:22 GMT  
		Size: 262.2 KB (262191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dcc8fe6b031dddb7ee69684824d72831849927f310d7a78c509de355dc75e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:21 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad2443021a6726dfc79be4f57e7f0f6ee1ff0584377c492703e027d379c085`  
		Last Modified: Fri, 22 Apr 2022 04:26:25 GMT  
		Size: 21.4 MB (21435296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:05ff07940a5ed666b30f0e9cb3e5989e3d0af92393950351c418c5ccc8703137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:57982240c0b1d9639b5d4017bd39fd04ffb6e1947f059b9bb2c46320879db806
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235830367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf1eab5ff47ea02c884e6f99e01b82106247185704ba244505d93fa6ec51b75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:41:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:41:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:41:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d81b4f14257aafe9c36754217f7b33e5594f7991bdc5fed442f3e351818ca6`  
		Last Modified: Fri, 22 Apr 2022 03:54:26 GMT  
		Size: 74.5 MB (74494199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86ee117572ea9ab37045a8143bd74f2c6fc866407f2c1b855fef3c348bec9f6`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 262.2 KB (262250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc056e4b5fb80b3e3a36e14d46061812f16e11166015dfbf5c8e9f911b4bc5e0`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a725f33deb8c6696fb2fe8f21c3fe0f20e6598f23354c10b3d1953701fe651`  
		Last Modified: Fri, 22 Apr 2022 03:54:18 GMT  
		Size: 22.1 MB (22113636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:226fa8b063571c73b4edede044f3a5c5dd59c24dcd749be5af219ae29ab60229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224032026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea80bb6394b0a866f1da8a2d6bbf18c448a676b6ac18e4c23c17c3926c256d41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:14:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04358f3e939d7f9f6a53c0ecd2c599e6321d2b4b0c0e9978c2dc6f05632e9711`  
		Last Modified: Fri, 22 Apr 2022 04:26:32 GMT  
		Size: 68.6 MB (68617910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cf32eefb7bf397b5f31ea8c519a7b26f428c65adf974fcbef5723a3b4d940`  
		Last Modified: Fri, 22 Apr 2022 04:26:22 GMT  
		Size: 262.2 KB (262191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dcc8fe6b031dddb7ee69684824d72831849927f310d7a78c509de355dc75e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:21 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad2443021a6726dfc79be4f57e7f0f6ee1ff0584377c492703e027d379c085`  
		Last Modified: Fri, 22 Apr 2022 04:26:25 GMT  
		Size: 21.4 MB (21435296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:05ff07940a5ed666b30f0e9cb3e5989e3d0af92393950351c418c5ccc8703137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:57982240c0b1d9639b5d4017bd39fd04ffb6e1947f059b9bb2c46320879db806
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235830367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf1eab5ff47ea02c884e6f99e01b82106247185704ba244505d93fa6ec51b75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:41:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:41:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:41:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d81b4f14257aafe9c36754217f7b33e5594f7991bdc5fed442f3e351818ca6`  
		Last Modified: Fri, 22 Apr 2022 03:54:26 GMT  
		Size: 74.5 MB (74494199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86ee117572ea9ab37045a8143bd74f2c6fc866407f2c1b855fef3c348bec9f6`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 262.2 KB (262250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc056e4b5fb80b3e3a36e14d46061812f16e11166015dfbf5c8e9f911b4bc5e0`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a725f33deb8c6696fb2fe8f21c3fe0f20e6598f23354c10b3d1953701fe651`  
		Last Modified: Fri, 22 Apr 2022 03:54:18 GMT  
		Size: 22.1 MB (22113636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:226fa8b063571c73b4edede044f3a5c5dd59c24dcd749be5af219ae29ab60229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224032026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea80bb6394b0a866f1da8a2d6bbf18c448a676b6ac18e4c23c17c3926c256d41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:14:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04358f3e939d7f9f6a53c0ecd2c599e6321d2b4b0c0e9978c2dc6f05632e9711`  
		Last Modified: Fri, 22 Apr 2022 04:26:32 GMT  
		Size: 68.6 MB (68617910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cf32eefb7bf397b5f31ea8c519a7b26f428c65adf974fcbef5723a3b4d940`  
		Last Modified: Fri, 22 Apr 2022 04:26:22 GMT  
		Size: 262.2 KB (262191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dcc8fe6b031dddb7ee69684824d72831849927f310d7a78c509de355dc75e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:21 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad2443021a6726dfc79be4f57e7f0f6ee1ff0584377c492703e027d379c085`  
		Last Modified: Fri, 22 Apr 2022 04:26:25 GMT  
		Size: 21.4 MB (21435296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:2169c63744b457dcc8b54f4720ab942724793556eb1742fe7c788db7768b413c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c644630aa2cadfb39da6be16c872c066e583724bb601c338cd9f9bba235c12bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138958088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cce7931771f1d143f583c2a02af3a0452f1f4abd91a6da08f4bdab2b99b69347`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b83332170f36ac3ef63f5c734064a19e83a0fbe29b270b049d43eeb788a13098
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133714483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d060b99544b550aa1a22f91448532c36ef4725081b3ff9ef54f8d42f28807d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:2169c63744b457dcc8b54f4720ab942724793556eb1742fe7c788db7768b413c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:c644630aa2cadfb39da6be16c872c066e583724bb601c338cd9f9bba235c12bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138958088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cce7931771f1d143f583c2a02af3a0452f1f4abd91a6da08f4bdab2b99b69347`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b83332170f36ac3ef63f5c734064a19e83a0fbe29b270b049d43eeb788a13098
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133714483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d060b99544b550aa1a22f91448532c36ef4725081b3ff9ef54f8d42f28807d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:2fb75f496f44cebba615ca09a7c8b89be836ee40d88fe0ba3e02c787f2ce0fc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:1ee3ad3ffb633974159613107bbadc7f6dd7ad5807c60e139922774fe90e780b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330799106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f77c5f173ec4f3c66c94951fabd1f99f7111e3cb9bfc7aea69a7563c30d0c15`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:41:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:41:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:41:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:41:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:41:38 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 03:41:38 GMT
ENV ROS2_DISTRO=galactic
# Fri, 22 Apr 2022 03:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:14 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d81b4f14257aafe9c36754217f7b33e5594f7991bdc5fed442f3e351818ca6`  
		Last Modified: Fri, 22 Apr 2022 03:54:26 GMT  
		Size: 74.5 MB (74494199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86ee117572ea9ab37045a8143bd74f2c6fc866407f2c1b855fef3c348bec9f6`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 262.2 KB (262250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc056e4b5fb80b3e3a36e14d46061812f16e11166015dfbf5c8e9f911b4bc5e0`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a725f33deb8c6696fb2fe8f21c3fe0f20e6598f23354c10b3d1953701fe651`  
		Last Modified: Fri, 22 Apr 2022 03:54:18 GMT  
		Size: 22.1 MB (22113636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35397945785dd434ec219e89250b0f82e33f7e60fa1ecaece9dc3c9e24bc0898`  
		Last Modified: Fri, 22 Apr 2022 03:54:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec5c0b2de935b90b5d54f02de899a12d4160855583ae6d65db5c6584a36dbe9`  
		Last Modified: Fri, 22 Apr 2022 03:54:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679fbb730a3136b74b5877ac3a03ee66cece62f0068afe23aae6173aad122c88`  
		Last Modified: Fri, 22 Apr 2022 03:54:54 GMT  
		Size: 78.6 MB (78597460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e57be180fb5ee836d1688d5d00f7ccf15ab87060b5d7f177b04ad4ca3c4ae4e`  
		Last Modified: Fri, 22 Apr 2022 03:54:43 GMT  
		Size: 16.4 MB (16370653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a40b523eed521aa1ac1f804bef4890d0051443a53b28d5d17dcf210e8e3098`  
		Last Modified: Fri, 22 Apr 2022 03:54:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cd79d7851bd1c39dbfd8af2ffd0adafd2f0581d6b80a2dd27588e8055f674df5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318030159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee43779417d83dbf623f1e138945a236116345cb844cd66d5618399805fa365`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:14:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:14:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:14:40 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 04:14:41 GMT
ENV ROS2_DISTRO=galactic
# Fri, 22 Apr 2022 04:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04358f3e939d7f9f6a53c0ecd2c599e6321d2b4b0c0e9978c2dc6f05632e9711`  
		Last Modified: Fri, 22 Apr 2022 04:26:32 GMT  
		Size: 68.6 MB (68617910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cf32eefb7bf397b5f31ea8c519a7b26f428c65adf974fcbef5723a3b4d940`  
		Last Modified: Fri, 22 Apr 2022 04:26:22 GMT  
		Size: 262.2 KB (262191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dcc8fe6b031dddb7ee69684824d72831849927f310d7a78c509de355dc75e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:21 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad2443021a6726dfc79be4f57e7f0f6ee1ff0584377c492703e027d379c085`  
		Last Modified: Fri, 22 Apr 2022 04:26:25 GMT  
		Size: 21.4 MB (21435296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f28ef04b4d186588a9d9764edc738cfe8e9afe7321f25cb1c909c4629811219`  
		Last Modified: Fri, 22 Apr 2022 04:26:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75db092a91e158f55d3ac36e2236c42c010a81238041ca129c0b8b7b6521ed81`  
		Last Modified: Fri, 22 Apr 2022 04:27:02 GMT  
		Size: 78.3 MB (78327585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2421d86da9c969395c3851f7e6024ad76ac3b3f84d42da6c239e3a5e9c84083`  
		Last Modified: Fri, 22 Apr 2022 04:26:50 GMT  
		Size: 15.7 MB (15670078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96431377503e489059103f86be358b18c448ffb4a71af36425dfb0ebcd2a6e5c`  
		Last Modified: Fri, 22 Apr 2022 04:26:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:2fb75f496f44cebba615ca09a7c8b89be836ee40d88fe0ba3e02c787f2ce0fc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:1ee3ad3ffb633974159613107bbadc7f6dd7ad5807c60e139922774fe90e780b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330799106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f77c5f173ec4f3c66c94951fabd1f99f7111e3cb9bfc7aea69a7563c30d0c15`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:41:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:41:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:41:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:41:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:41:38 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 03:41:38 GMT
ENV ROS2_DISTRO=galactic
# Fri, 22 Apr 2022 03:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:14 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d81b4f14257aafe9c36754217f7b33e5594f7991bdc5fed442f3e351818ca6`  
		Last Modified: Fri, 22 Apr 2022 03:54:26 GMT  
		Size: 74.5 MB (74494199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86ee117572ea9ab37045a8143bd74f2c6fc866407f2c1b855fef3c348bec9f6`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 262.2 KB (262250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc056e4b5fb80b3e3a36e14d46061812f16e11166015dfbf5c8e9f911b4bc5e0`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a725f33deb8c6696fb2fe8f21c3fe0f20e6598f23354c10b3d1953701fe651`  
		Last Modified: Fri, 22 Apr 2022 03:54:18 GMT  
		Size: 22.1 MB (22113636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35397945785dd434ec219e89250b0f82e33f7e60fa1ecaece9dc3c9e24bc0898`  
		Last Modified: Fri, 22 Apr 2022 03:54:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec5c0b2de935b90b5d54f02de899a12d4160855583ae6d65db5c6584a36dbe9`  
		Last Modified: Fri, 22 Apr 2022 03:54:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679fbb730a3136b74b5877ac3a03ee66cece62f0068afe23aae6173aad122c88`  
		Last Modified: Fri, 22 Apr 2022 03:54:54 GMT  
		Size: 78.6 MB (78597460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e57be180fb5ee836d1688d5d00f7ccf15ab87060b5d7f177b04ad4ca3c4ae4e`  
		Last Modified: Fri, 22 Apr 2022 03:54:43 GMT  
		Size: 16.4 MB (16370653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a40b523eed521aa1ac1f804bef4890d0051443a53b28d5d17dcf210e8e3098`  
		Last Modified: Fri, 22 Apr 2022 03:54:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cd79d7851bd1c39dbfd8af2ffd0adafd2f0581d6b80a2dd27588e8055f674df5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318030159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee43779417d83dbf623f1e138945a236116345cb844cd66d5618399805fa365`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:14:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:14:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:14:40 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 04:14:41 GMT
ENV ROS2_DISTRO=galactic
# Fri, 22 Apr 2022 04:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04358f3e939d7f9f6a53c0ecd2c599e6321d2b4b0c0e9978c2dc6f05632e9711`  
		Last Modified: Fri, 22 Apr 2022 04:26:32 GMT  
		Size: 68.6 MB (68617910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cf32eefb7bf397b5f31ea8c519a7b26f428c65adf974fcbef5723a3b4d940`  
		Last Modified: Fri, 22 Apr 2022 04:26:22 GMT  
		Size: 262.2 KB (262191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dcc8fe6b031dddb7ee69684824d72831849927f310d7a78c509de355dc75e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:21 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad2443021a6726dfc79be4f57e7f0f6ee1ff0584377c492703e027d379c085`  
		Last Modified: Fri, 22 Apr 2022 04:26:25 GMT  
		Size: 21.4 MB (21435296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f28ef04b4d186588a9d9764edc738cfe8e9afe7321f25cb1c909c4629811219`  
		Last Modified: Fri, 22 Apr 2022 04:26:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75db092a91e158f55d3ac36e2236c42c010a81238041ca129c0b8b7b6521ed81`  
		Last Modified: Fri, 22 Apr 2022 04:27:02 GMT  
		Size: 78.3 MB (78327585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2421d86da9c969395c3851f7e6024ad76ac3b3f84d42da6c239e3a5e9c84083`  
		Last Modified: Fri, 22 Apr 2022 04:26:50 GMT  
		Size: 15.7 MB (15670078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96431377503e489059103f86be358b18c448ffb4a71af36425dfb0ebcd2a6e5c`  
		Last Modified: Fri, 22 Apr 2022 04:26:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:f7299f4eb820c59adaeb9c16af428ac3e0aab0ff38735cd453145c4c4cbf79d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:18e9dbacc08da9636fe5c515d7303715d0e87d15a53879ccab9d979087ba9a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251846325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c645eb93f5e52feb828db0e9fa5f313ca3c35a01dd8ebff251680537d6ad3403`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2f629aab5a540a63cdbc508dda1e8c60d49c4eeb5d94de9f4998b41b93fc8da5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227242523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5a452b850177955c2793a3f03ec97ac920e348c663671a2f538cafff7011118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:d837dab96c205dd9328ce07529cb0c2515736b2c941974a15ed071e2060e7a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:b35e906f707bf988db588f95ca6370e62514d104a193a57b4632649a0d97b48c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437394244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5023ff407aa1e7f107544b46c999a8edce6403d120be868f5edb7d852da0eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f74aae7c041fcdbca8b5d0c1e96e06ef05af66145f8f942c371f0a9f1d6e7e09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385904838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca9d5b1d6627a3b25f3cbd8d26e71b1eb836ad546306352eac8ceb6bbfacdcf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ef4ec58b9955078e592b2a50d64c7f8018c28cc9c0253b94f3cda56041dc5f9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411582050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3813e667132713e7951661e3eee6e90e0adbce9e3577cd548e30071b47a357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:01024e90f152b7d3b02eb8a0431b1b452b6e9b8b2ea33380240eb5829300614f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:b3404f2853827d7efc1e557ee67ecec5abad6c4be9b4ef8ecf5fb030e9a4f454
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742710927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f2b2bc1d75b72a2da3c58631a301ce9812d3a552f21af6f8137544a5d409b9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493c771b079d789db9df9583325355027638af6b25d95d4a937ce930de755c04`  
		Last Modified: Fri, 22 Apr 2022 03:49:28 GMT  
		Size: 305.3 MB (305316683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:36d1b962367d2b70a973ffdf7fcc829607167412f0d16f2b082190cc363ec216
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645948490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:260bce6c2fd5fead0d53c6d6fb71998c85e9480d2563d97c556eeaeb585a176c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e2c5cd63790109b35d5d0faa358a07e77cca90743d1072ca95aa3942194a01`  
		Last Modified: Sat, 23 Apr 2022 01:21:49 GMT  
		Size: 260.0 MB (260043652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f12b260de41cbd5f844f154c3328d7032e432f429913d54af82ec218c0f5732b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (702986156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06ae26027ffeb1a71eb82f3cfd5bcce58833efe79e0c7c9ad08ed418c4f9b354`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8dd41134e5d01c61820548bb8e5800dfd75cd3deae4abe34f08a21b5c53968`  
		Last Modified: Fri, 22 Apr 2022 04:21:34 GMT  
		Size: 291.4 MB (291404106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:01024e90f152b7d3b02eb8a0431b1b452b6e9b8b2ea33380240eb5829300614f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b3404f2853827d7efc1e557ee67ecec5abad6c4be9b4ef8ecf5fb030e9a4f454
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742710927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f2b2bc1d75b72a2da3c58631a301ce9812d3a552f21af6f8137544a5d409b9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493c771b079d789db9df9583325355027638af6b25d95d4a937ce930de755c04`  
		Last Modified: Fri, 22 Apr 2022 03:49:28 GMT  
		Size: 305.3 MB (305316683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:36d1b962367d2b70a973ffdf7fcc829607167412f0d16f2b082190cc363ec216
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645948490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:260bce6c2fd5fead0d53c6d6fb71998c85e9480d2563d97c556eeaeb585a176c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e2c5cd63790109b35d5d0faa358a07e77cca90743d1072ca95aa3942194a01`  
		Last Modified: Sat, 23 Apr 2022 01:21:49 GMT  
		Size: 260.0 MB (260043652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f12b260de41cbd5f844f154c3328d7032e432f429913d54af82ec218c0f5732b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (702986156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06ae26027ffeb1a71eb82f3cfd5bcce58833efe79e0c7c9ad08ed418c4f9b354`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8dd41134e5d01c61820548bb8e5800dfd75cd3deae4abe34f08a21b5c53968`  
		Last Modified: Fri, 22 Apr 2022 04:21:34 GMT  
		Size: 291.4 MB (291404106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:96777be5f3eefb281999d0d174e5e3fddcb84b94ef979ef5384f412a16070b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:a28bc3f892f1dfeecae7a00ba6304b00add7a4f48d9ecc1357d7bd5a3f87a2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448477280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec5677d8005df5c0680c12d81e6e284c12cbdf56cd93577cbf4d460cf52bd33`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ce09845a35fb485ffe49a62e58ecd3d528a9aeb7429bdf7fd6941e6eb3ffa`  
		Last Modified: Fri, 22 Apr 2022 03:48:30 GMT  
		Size: 11.1 MB (11083036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:fddf912a33c82b1543471eae076ad06cf16b35a42e3148bb26fe1a6c9b4f54ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396028177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ec100476c77a1d1449d13f1fef83b0aa56ae785d5cfa2f1916d65d1ef420a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:59:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4e98b064e5e1e5a43843cc6fa030e1e15c6870aba0bde15440c84e01a8b72d`  
		Last Modified: Sat, 23 Apr 2022 01:18:52 GMT  
		Size: 10.1 MB (10123339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9a9e3ee3227232758bccb1d3fdf9d549d273aa592bb8e91b604709ddc8560cb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422316119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fd080112e8b140a1f7f8bdc44ec527dca5d2546246cf064aa9ce9d86308aeb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20abf96d320289bcf7aaa0d966c1f356ae4f571e3954978baa1dff37d0ccde36`  
		Last Modified: Fri, 22 Apr 2022 04:20:34 GMT  
		Size: 10.7 MB (10734069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:96777be5f3eefb281999d0d174e5e3fddcb84b94ef979ef5384f412a16070b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:a28bc3f892f1dfeecae7a00ba6304b00add7a4f48d9ecc1357d7bd5a3f87a2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448477280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec5677d8005df5c0680c12d81e6e284c12cbdf56cd93577cbf4d460cf52bd33`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ce09845a35fb485ffe49a62e58ecd3d528a9aeb7429bdf7fd6941e6eb3ffa`  
		Last Modified: Fri, 22 Apr 2022 03:48:30 GMT  
		Size: 11.1 MB (11083036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:fddf912a33c82b1543471eae076ad06cf16b35a42e3148bb26fe1a6c9b4f54ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396028177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ec100476c77a1d1449d13f1fef83b0aa56ae785d5cfa2f1916d65d1ef420a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:59:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4e98b064e5e1e5a43843cc6fa030e1e15c6870aba0bde15440c84e01a8b72d`  
		Last Modified: Sat, 23 Apr 2022 01:18:52 GMT  
		Size: 10.1 MB (10123339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9a9e3ee3227232758bccb1d3fdf9d549d273aa592bb8e91b604709ddc8560cb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422316119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fd080112e8b140a1f7f8bdc44ec527dca5d2546246cf064aa9ce9d86308aeb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20abf96d320289bcf7aaa0d966c1f356ae4f571e3954978baa1dff37d0ccde36`  
		Last Modified: Fri, 22 Apr 2022 04:20:34 GMT  
		Size: 10.7 MB (10734069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:d837dab96c205dd9328ce07529cb0c2515736b2c941974a15ed071e2060e7a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b35e906f707bf988db588f95ca6370e62514d104a193a57b4632649a0d97b48c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437394244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5023ff407aa1e7f107544b46c999a8edce6403d120be868f5edb7d852da0eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:f74aae7c041fcdbca8b5d0c1e96e06ef05af66145f8f942c371f0a9f1d6e7e09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385904838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca9d5b1d6627a3b25f3cbd8d26e71b1eb836ad546306352eac8ceb6bbfacdcf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ef4ec58b9955078e592b2a50d64c7f8018c28cc9c0253b94f3cda56041dc5f9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411582050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3813e667132713e7951661e3eee6e90e0adbce9e3577cd548e30071b47a357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:d837dab96c205dd9328ce07529cb0c2515736b2c941974a15ed071e2060e7a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b35e906f707bf988db588f95ca6370e62514d104a193a57b4632649a0d97b48c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437394244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5023ff407aa1e7f107544b46c999a8edce6403d120be868f5edb7d852da0eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f74aae7c041fcdbca8b5d0c1e96e06ef05af66145f8f942c371f0a9f1d6e7e09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385904838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca9d5b1d6627a3b25f3cbd8d26e71b1eb836ad546306352eac8ceb6bbfacdcf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ef4ec58b9955078e592b2a50d64c7f8018c28cc9c0253b94f3cda56041dc5f9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411582050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3813e667132713e7951661e3eee6e90e0adbce9e3577cd548e30071b47a357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:247bda8ab0b5b626affd87b426d107849e2974c1e51fab891a93c65ee2a75954
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:df25ed094291a1fb6871268725546bdaec1755a6adcc3e01006291f069ed4c77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291879268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da5a74700fa30db918ce7f3f12af76aa76fd9a048ff3df2d2598696f78ffe3f6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:14465a61f6a15d0fc5e2c8f830b8e4a01f672c3b7449b9e1dfa17cabb67f442b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266167201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24715a8b88a636f779248751c36e79e2e95ee987dba6284ea4f484a2252c607d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9b7b6ce81005899ea2fefea035c323cf3e2fc4ad20c5393f873379bba2647340
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281224131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30cfb642e18d870ce7b704d1cbf74b66acfe4936a0b8837e3f067cee3257489`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:247bda8ab0b5b626affd87b426d107849e2974c1e51fab891a93c65ee2a75954
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:df25ed094291a1fb6871268725546bdaec1755a6adcc3e01006291f069ed4c77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291879268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da5a74700fa30db918ce7f3f12af76aa76fd9a048ff3df2d2598696f78ffe3f6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:14465a61f6a15d0fc5e2c8f830b8e4a01f672c3b7449b9e1dfa17cabb67f442b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266167201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24715a8b88a636f779248751c36e79e2e95ee987dba6284ea4f484a2252c607d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9b7b6ce81005899ea2fefea035c323cf3e2fc4ad20c5393f873379bba2647340
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281224131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30cfb642e18d870ce7b704d1cbf74b66acfe4936a0b8837e3f067cee3257489`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:0da29824955ada3c4e46a1fc93bd3ff9008e124ac632e123989a3c896a0fc181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:62e0f0bf5659f14e229c216fa8b63e1ee9d2ca697ad8a5471bfe157b9957efad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343021947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd733d2da3cc8a934cace2a21423ed6c30c11016a16c493a06b9b3f312039b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:074568bdd51220fc0cd8418cf81ad0c619abf863b220816ef618324bfdfd45b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.7 MB (288657312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f5d828da189218e815fb24701c5c0e51c071b40087f44388b60005180a794a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f761181463424d5e410690c40d811c9d9274554c1b753a522491b4717d606acb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322035191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a04fc513eaccebdfab28a02b6497fca8d6743cf0e99bd96367e2445db44a72`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:ed176154dffda539d5367e97152fd003610f3559ae7e962c3120144d72e9e24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:ab69286a981b4c72f6cfc5c3b5b915d7976c67edf8350649071ecc6a1855f920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834986866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4e4bba5021550a163834d0d889b8f07daafecdaf9de04b4e27ca6f13665025`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:36:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92599f66529a813a6e3e49ab12cf914bb5e22f6f03eff38e96f0b8cb317b249`  
		Last Modified: Fri, 22 Apr 2022 03:52:11 GMT  
		Size: 492.0 MB (491964919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:bc97aa69ad149938b4a376ee803eb901d86a2d738eea6999a3b21e9275c00b20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.6 MB (725582608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd907b1c190d5149ef8e424dc3f3be4c058b3998da14ca0ef1cb4a1e6598edaf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb032a70fb376f95cdc33bcd0a48aff332773c86ad12bb719dc31feab44b5c9`  
		Last Modified: Sat, 23 Apr 2022 01:30:10 GMT  
		Size: 436.9 MB (436925296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:822d55d8e5db88b18a8402842e71b6281321f07469affbc499bfa930ce81dbb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.5 MB (784528201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d61056ee090fdeb21e163357da8bc408b4eaaf09b0d3e55c5d87489ce6dcb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eb63c1f2c9e055fd5f1dc6867393368659b889d9ee88fe4917338270821237`  
		Last Modified: Fri, 22 Apr 2022 04:24:13 GMT  
		Size: 462.5 MB (462493010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:8ad82eff31eaa1d0bf1d9e9e564bcf1d6f001124a6c768ff17ad74f35b91e0f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:25bc6ce5fdfefee48e015f60e641910a0142999ad6e4332ae4bf3818dc8bf497
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.5 MB (951517214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9764e88e4b84531e3e1aa2b08bb398c9693f5be42ee0743dfe1a553040854f3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:37:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:37:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 17:37:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 17:38:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:38:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 17:38:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 17:38:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:38:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:39:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 20 Apr 2022 17:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:41:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20546aaa06f50802eafdb39e7339d4cb6230c7a1aff32a53c46d1fcfed8f2dd5`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 10.9 MB (10892097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abde7f24de9cf0bbb2249385441601015b239338b7901eae3402cb42a98c589`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4f8c5429cab550330c262feb633f708f9eda06ab0962fa784c88a9c3459a`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8609835955c8073fb8ee41d1c9ebb686c08c5a154f81dc42e1ee92614d6e430`  
		Last Modified: Wed, 20 Apr 2022 17:43:31 GMT  
		Size: 239.2 MB (239162184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb06026309bf4ee95de3a56281f392cddaad08a74c5056617cee6a3cbad0840`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757a381d58433d12adbc8267c4306c48e05ceab27e9b7180e6ab5153115398a9`  
		Last Modified: Wed, 20 Apr 2022 17:43:51 GMT  
		Size: 86.6 MB (86566693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d2e540aad82640f395c83b534034224c4743c463281a9308bcd39e755a9a5`  
		Last Modified: Wed, 20 Apr 2022 17:43:39 GMT  
		Size: 309.3 KB (309290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc64f783db31ecba0dea771f5c67d54898bd9e111176ecd00620deaa53fef6e`  
		Last Modified: Wed, 20 Apr 2022 17:43:49 GMT  
		Size: 76.0 MB (75976251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a6c84da7010552c141b5d0c478700dd9362ce1ff0a16729b967a26cfe6b941`  
		Last Modified: Wed, 20 Apr 2022 17:45:22 GMT  
		Size: 488.2 MB (488171305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:25b6fe2a0e3dfdddf6d36c32b27206b68b4ae4cb544a4fda27922baa7ef31bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.7 MB (867713663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bcf21208468124b3285b34c0276748127e9ae21c28c8082af342ed7ce0e62b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:10:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:10:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 12:10:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 12:10:22 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:10:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 12:10:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 12:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:11:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 12:11:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 12:11:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:12:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 20 Apr 2022 12:13:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:16:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957d218911547e664ee734939dc71ad089b29ed94b50f538786d667373e1ce5`  
		Last Modified: Wed, 20 Apr 2022 12:18:50 GMT  
		Size: 10.7 MB (10688204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c217f5a5971a62fad5aac5564915eaf89c57b2110a7751a364f5a0de02dd7`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a549feaf8502a671617c04bc2c2a084e6374b096bd615bebf4d2b3278be0a`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a05822887f56bc9d0b9364d7c755b5baee6c94b00f61dd5c41b4c2392919797`  
		Last Modified: Wed, 20 Apr 2022 12:19:19 GMT  
		Size: 184.4 MB (184369896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8501994f2ad5e8e01905fad8c5f1491a035971eab743a788c7208cf18255c4e`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36c64b99b0defab15ab0ce0f85dbf6fbab02bd969287c79becce5d9293059c`  
		Last Modified: Wed, 20 Apr 2022 12:19:38 GMT  
		Size: 84.4 MB (84352350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359920e3958bfbe6523bec5a0c24d8479e58e68ab41c3c437aa9806e83e776e`  
		Last Modified: Wed, 20 Apr 2022 12:19:27 GMT  
		Size: 309.2 KB (309235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22341ca497d2ab03ede7e0d29948509d06168bfff83be501fc2c9fb1499be`  
		Last Modified: Wed, 20 Apr 2022 12:19:37 GMT  
		Size: 73.9 MB (73865013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bc4fe6b32b74a770b835d7ef94154e208ca4d9d3c236f06b6e38fe5a5a75ce`  
		Last Modified: Wed, 20 Apr 2022 12:21:03 GMT  
		Size: 464.9 MB (464898859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:ed176154dffda539d5367e97152fd003610f3559ae7e962c3120144d72e9e24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:ab69286a981b4c72f6cfc5c3b5b915d7976c67edf8350649071ecc6a1855f920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834986866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4e4bba5021550a163834d0d889b8f07daafecdaf9de04b4e27ca6f13665025`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:36:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92599f66529a813a6e3e49ab12cf914bb5e22f6f03eff38e96f0b8cb317b249`  
		Last Modified: Fri, 22 Apr 2022 03:52:11 GMT  
		Size: 492.0 MB (491964919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:bc97aa69ad149938b4a376ee803eb901d86a2d738eea6999a3b21e9275c00b20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.6 MB (725582608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd907b1c190d5149ef8e424dc3f3be4c058b3998da14ca0ef1cb4a1e6598edaf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb032a70fb376f95cdc33bcd0a48aff332773c86ad12bb719dc31feab44b5c9`  
		Last Modified: Sat, 23 Apr 2022 01:30:10 GMT  
		Size: 436.9 MB (436925296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:822d55d8e5db88b18a8402842e71b6281321f07469affbc499bfa930ce81dbb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.5 MB (784528201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d61056ee090fdeb21e163357da8bc408b4eaaf09b0d3e55c5d87489ce6dcb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eb63c1f2c9e055fd5f1dc6867393368659b889d9ee88fe4917338270821237`  
		Last Modified: Fri, 22 Apr 2022 04:24:13 GMT  
		Size: 462.5 MB (462493010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:d53671120c79755fc3bc654b8984e155b1902736cde6bbfa7dd10e629c49f877
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:82adffa092e98d53cac94a9ecb55ba7569efc8f0f5d22fa619f93ce70eb50a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358880748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e0ca8e38ae15069727b4c1507435dfe3fb53c865c6ab323f807fd32afdec7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f093d22dbe5877606fa8a0bb7ab4ff9f764a797720db05f3891f492ba89135`  
		Last Modified: Fri, 22 Apr 2022 03:50:46 GMT  
		Size: 15.9 MB (15858801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:cc8b94ba7be48707d801a8625d42f5719f34ace16f442de9b409a4da99645dce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302721758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3be1b316388d7521caddb1b63790c6f62911e0e387087508a86d6a014ea2a41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:08:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8713ba4b0281ed1eed08b6b88dd2382461ef68e4919ad6e671af93353b37d5b9`  
		Last Modified: Sat, 23 Apr 2022 01:25:28 GMT  
		Size: 14.1 MB (14064446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e688ed73e138f25890349e5090c1c3b0c970ce916148b160d74bdae7f87174c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337482921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b02bf96a11e1a6d842331a5bd039931f13a1c2437d6169445c1feb2d4dc56e1d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:05:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ad38acc3207d37bdbd042778978ce56aeb0844496c6d6b4fbe085abcd61151`  
		Last Modified: Fri, 22 Apr 2022 04:22:54 GMT  
		Size: 15.4 MB (15447730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:639cbd7dd6e31741d5501387d4b4d3ea14184abe76b63a3b54d0da46bca4ae9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:06f11bae1fe6d88435a4f3fd50f68714f82ac481556a5fe64d7728626afe6395
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.8 MB (484792573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df3ed63c705dfd05177d123ca4d5a37b56dbeede4cfc71c9ddfd54b46e0c72c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:37:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:37:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 17:37:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 17:38:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:38:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 17:38:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 17:38:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:38:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:39:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 20 Apr 2022 17:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20546aaa06f50802eafdb39e7339d4cb6230c7a1aff32a53c46d1fcfed8f2dd5`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 10.9 MB (10892097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abde7f24de9cf0bbb2249385441601015b239338b7901eae3402cb42a98c589`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4f8c5429cab550330c262feb633f708f9eda06ab0962fa784c88a9c3459a`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8609835955c8073fb8ee41d1c9ebb686c08c5a154f81dc42e1ee92614d6e430`  
		Last Modified: Wed, 20 Apr 2022 17:43:31 GMT  
		Size: 239.2 MB (239162184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb06026309bf4ee95de3a56281f392cddaad08a74c5056617cee6a3cbad0840`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757a381d58433d12adbc8267c4306c48e05ceab27e9b7180e6ab5153115398a9`  
		Last Modified: Wed, 20 Apr 2022 17:43:51 GMT  
		Size: 86.6 MB (86566693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d2e540aad82640f395c83b534034224c4743c463281a9308bcd39e755a9a5`  
		Last Modified: Wed, 20 Apr 2022 17:43:39 GMT  
		Size: 309.3 KB (309290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc64f783db31ecba0dea771f5c67d54898bd9e111176ecd00620deaa53fef6e`  
		Last Modified: Wed, 20 Apr 2022 17:43:49 GMT  
		Size: 76.0 MB (75976251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1c560921f8011622c11605269becc4a75f29225fe293f61872f0046836466a`  
		Last Modified: Wed, 20 Apr 2022 17:44:01 GMT  
		Size: 21.4 MB (21446664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f6d9402dd9ab9325e630216c0891b72ea6f7be615d81b3d353d2d87dcb0a3528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423920584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86513fad1e0a77e9431d687d44981867b263681a71c599265f41c15ffa14429`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:10:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:10:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 12:10:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 12:10:22 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:10:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 12:10:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 12:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:11:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 12:11:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 12:11:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:12:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 20 Apr 2022 12:13:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957d218911547e664ee734939dc71ad089b29ed94b50f538786d667373e1ce5`  
		Last Modified: Wed, 20 Apr 2022 12:18:50 GMT  
		Size: 10.7 MB (10688204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c217f5a5971a62fad5aac5564915eaf89c57b2110a7751a364f5a0de02dd7`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a549feaf8502a671617c04bc2c2a084e6374b096bd615bebf4d2b3278be0a`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a05822887f56bc9d0b9364d7c755b5baee6c94b00f61dd5c41b4c2392919797`  
		Last Modified: Wed, 20 Apr 2022 12:19:19 GMT  
		Size: 184.4 MB (184369896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8501994f2ad5e8e01905fad8c5f1491a035971eab743a788c7208cf18255c4e`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36c64b99b0defab15ab0ce0f85dbf6fbab02bd969287c79becce5d9293059c`  
		Last Modified: Wed, 20 Apr 2022 12:19:38 GMT  
		Size: 84.4 MB (84352350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359920e3958bfbe6523bec5a0c24d8479e58e68ab41c3c437aa9806e83e776e`  
		Last Modified: Wed, 20 Apr 2022 12:19:27 GMT  
		Size: 309.2 KB (309235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22341ca497d2ab03ede7e0d29948509d06168bfff83be501fc2c9fb1499be`  
		Last Modified: Wed, 20 Apr 2022 12:19:37 GMT  
		Size: 73.9 MB (73865013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd96d96d99154147eebbce9635acab9f6a43ffeac0ccf758ad22469b3c6fc15`  
		Last Modified: Wed, 20 Apr 2022 12:19:49 GMT  
		Size: 21.1 MB (21105780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:d53671120c79755fc3bc654b8984e155b1902736cde6bbfa7dd10e629c49f877
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:82adffa092e98d53cac94a9ecb55ba7569efc8f0f5d22fa619f93ce70eb50a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358880748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e0ca8e38ae15069727b4c1507435dfe3fb53c865c6ab323f807fd32afdec7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f093d22dbe5877606fa8a0bb7ab4ff9f764a797720db05f3891f492ba89135`  
		Last Modified: Fri, 22 Apr 2022 03:50:46 GMT  
		Size: 15.9 MB (15858801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:cc8b94ba7be48707d801a8625d42f5719f34ace16f442de9b409a4da99645dce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302721758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3be1b316388d7521caddb1b63790c6f62911e0e387087508a86d6a014ea2a41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:08:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8713ba4b0281ed1eed08b6b88dd2382461ef68e4919ad6e671af93353b37d5b9`  
		Last Modified: Sat, 23 Apr 2022 01:25:28 GMT  
		Size: 14.1 MB (14064446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e688ed73e138f25890349e5090c1c3b0c970ce916148b160d74bdae7f87174c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337482921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b02bf96a11e1a6d842331a5bd039931f13a1c2437d6169445c1feb2d4dc56e1d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:05:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ad38acc3207d37bdbd042778978ce56aeb0844496c6d6b4fbe085abcd61151`  
		Last Modified: Fri, 22 Apr 2022 04:22:54 GMT  
		Size: 15.4 MB (15447730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:0da29824955ada3c4e46a1fc93bd3ff9008e124ac632e123989a3c896a0fc181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:62e0f0bf5659f14e229c216fa8b63e1ee9d2ca697ad8a5471bfe157b9957efad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343021947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd733d2da3cc8a934cace2a21423ed6c30c11016a16c493a06b9b3f312039b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:074568bdd51220fc0cd8418cf81ad0c619abf863b220816ef618324bfdfd45b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.7 MB (288657312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f5d828da189218e815fb24701c5c0e51c071b40087f44388b60005180a794a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f761181463424d5e410690c40d811c9d9274554c1b753a522491b4717d606acb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322035191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a04fc513eaccebdfab28a02b6497fca8d6743cf0e99bd96367e2445db44a72`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:e8d3f1b71626a3c53aeb5a67fdf9363f35dc897f7d36bff8133c8b29bad08e24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:6b4406b04c3846197e0bd36ebd863516ccf681c16a0bee86361a33ef668549c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463345909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:920dd0639d765b1780c742f8ab16fc2f50932373bfde99d3bb475d7b813f7067`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:37:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:37:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 17:37:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 17:38:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:38:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 17:38:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 17:38:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:38:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:39:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 20 Apr 2022 17:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20546aaa06f50802eafdb39e7339d4cb6230c7a1aff32a53c46d1fcfed8f2dd5`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 10.9 MB (10892097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abde7f24de9cf0bbb2249385441601015b239338b7901eae3402cb42a98c589`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4f8c5429cab550330c262feb633f708f9eda06ab0962fa784c88a9c3459a`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8609835955c8073fb8ee41d1c9ebb686c08c5a154f81dc42e1ee92614d6e430`  
		Last Modified: Wed, 20 Apr 2022 17:43:31 GMT  
		Size: 239.2 MB (239162184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb06026309bf4ee95de3a56281f392cddaad08a74c5056617cee6a3cbad0840`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757a381d58433d12adbc8267c4306c48e05ceab27e9b7180e6ab5153115398a9`  
		Last Modified: Wed, 20 Apr 2022 17:43:51 GMT  
		Size: 86.6 MB (86566693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d2e540aad82640f395c83b534034224c4743c463281a9308bcd39e755a9a5`  
		Last Modified: Wed, 20 Apr 2022 17:43:39 GMT  
		Size: 309.3 KB (309290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc64f783db31ecba0dea771f5c67d54898bd9e111176ecd00620deaa53fef6e`  
		Last Modified: Wed, 20 Apr 2022 17:43:49 GMT  
		Size: 76.0 MB (75976251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:93dbc8057d883b94580a8234ec329cda459fea35afe75515fb0f9a61d8be3e83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.8 MB (402814804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd23d08ebda2ecf5c0c0951aace97a48e98f0e7ff9ff80bc25cb84f4d52d6288`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:10:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:10:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 12:10:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 12:10:22 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:10:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 12:10:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 12:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:11:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 12:11:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 12:11:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:12:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 20 Apr 2022 12:13:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957d218911547e664ee734939dc71ad089b29ed94b50f538786d667373e1ce5`  
		Last Modified: Wed, 20 Apr 2022 12:18:50 GMT  
		Size: 10.7 MB (10688204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c217f5a5971a62fad5aac5564915eaf89c57b2110a7751a364f5a0de02dd7`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a549feaf8502a671617c04bc2c2a084e6374b096bd615bebf4d2b3278be0a`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a05822887f56bc9d0b9364d7c755b5baee6c94b00f61dd5c41b4c2392919797`  
		Last Modified: Wed, 20 Apr 2022 12:19:19 GMT  
		Size: 184.4 MB (184369896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8501994f2ad5e8e01905fad8c5f1491a035971eab743a788c7208cf18255c4e`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36c64b99b0defab15ab0ce0f85dbf6fbab02bd969287c79becce5d9293059c`  
		Last Modified: Wed, 20 Apr 2022 12:19:38 GMT  
		Size: 84.4 MB (84352350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359920e3958bfbe6523bec5a0c24d8479e58e68ab41c3c437aa9806e83e776e`  
		Last Modified: Wed, 20 Apr 2022 12:19:27 GMT  
		Size: 309.2 KB (309235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22341ca497d2ab03ede7e0d29948509d06168bfff83be501fc2c9fb1499be`  
		Last Modified: Wed, 20 Apr 2022 12:19:37 GMT  
		Size: 73.9 MB (73865013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:0da29824955ada3c4e46a1fc93bd3ff9008e124ac632e123989a3c896a0fc181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:62e0f0bf5659f14e229c216fa8b63e1ee9d2ca697ad8a5471bfe157b9957efad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343021947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd733d2da3cc8a934cace2a21423ed6c30c11016a16c493a06b9b3f312039b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:074568bdd51220fc0cd8418cf81ad0c619abf863b220816ef618324bfdfd45b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.7 MB (288657312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f5d828da189218e815fb24701c5c0e51c071b40087f44388b60005180a794a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f761181463424d5e410690c40d811c9d9274554c1b753a522491b4717d606acb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322035191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a04fc513eaccebdfab28a02b6497fca8d6743cf0e99bd96367e2445db44a72`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:b43d6b6be3695f05583bb30d1814b5713a40786ea1d944b927dd07b43ae15823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:d44e2d917030a80e982ed14e0450d57be0a03baa9dc90d5810f8620707f157da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212171208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fa98b743825a049a552c2f66c918e1b3190587b8e8f26ae9e62bea74906cfa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:759a7388044e3bc9be3f1ac86e99c8bd00dfcb7ac8eeca5e5000b27a1b31b392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187358703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddea610d1c28befab92434a77103b3dc5cf55e0599fd4c1b9fa2f06eef62d453`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:09a1a1ee820322b54ee0b5757e4b62fffce13be4bed8646f6169b27392643643
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (204978121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df55e467ad20a0cd08e10d6c447177f88021735a54af168940f4548a0935e83a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:89d2d4a66f45461a687e24602ae35bce5ce102bccf86d41a7a1c9b6163cd6e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:84351d18f44271dd8a4ace0db9e9a7c7ffa02a108ff424b3abcd8b055312a296
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300493675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdddb757d3d82bc10e186b274307e6f5b72f5aeb6590ba010135f94263fd1881`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:37:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:37:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 17:37:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 17:37:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 17:38:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:38:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 17:38:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 17:38:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20546aaa06f50802eafdb39e7339d4cb6230c7a1aff32a53c46d1fcfed8f2dd5`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 10.9 MB (10892097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abde7f24de9cf0bbb2249385441601015b239338b7901eae3402cb42a98c589`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4f8c5429cab550330c262feb633f708f9eda06ab0962fa784c88a9c3459a`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8609835955c8073fb8ee41d1c9ebb686c08c5a154f81dc42e1ee92614d6e430`  
		Last Modified: Wed, 20 Apr 2022 17:43:31 GMT  
		Size: 239.2 MB (239162184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb06026309bf4ee95de3a56281f392cddaad08a74c5056617cee6a3cbad0840`  
		Last Modified: Wed, 20 Apr 2022 17:42:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3a167a3e4a34b48fdac018fdb84126e3a9ea5c99e0a51cda3cfa472cba4e59aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244288206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d559d174d4ed076af61ea7fde4dca79121305b27a81c85da84fb2ed1dd24c426`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:10:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:10:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 20 Apr 2022 12:10:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 20 Apr 2022 12:10:22 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:10:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 20 Apr 2022 12:10:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 20 Apr 2022 12:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:11:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 20 Apr 2022 12:11:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 20 Apr 2022 12:11:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957d218911547e664ee734939dc71ad089b29ed94b50f538786d667373e1ce5`  
		Last Modified: Wed, 20 Apr 2022 12:18:50 GMT  
		Size: 10.7 MB (10688204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c217f5a5971a62fad5aac5564915eaf89c57b2110a7751a364f5a0de02dd7`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a549feaf8502a671617c04bc2c2a084e6374b096bd615bebf4d2b3278be0a`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a05822887f56bc9d0b9364d7c755b5baee6c94b00f61dd5c41b4c2392919797`  
		Last Modified: Wed, 20 Apr 2022 12:19:19 GMT  
		Size: 184.4 MB (184369896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8501994f2ad5e8e01905fad8c5f1491a035971eab743a788c7208cf18255c4e`  
		Last Modified: Wed, 20 Apr 2022 12:18:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:b43d6b6be3695f05583bb30d1814b5713a40786ea1d944b927dd07b43ae15823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:d44e2d917030a80e982ed14e0450d57be0a03baa9dc90d5810f8620707f157da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212171208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fa98b743825a049a552c2f66c918e1b3190587b8e8f26ae9e62bea74906cfa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:759a7388044e3bc9be3f1ac86e99c8bd00dfcb7ac8eeca5e5000b27a1b31b392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187358703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddea610d1c28befab92434a77103b3dc5cf55e0599fd4c1b9fa2f06eef62d453`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:09a1a1ee820322b54ee0b5757e4b62fffce13be4bed8646f6169b27392643643
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (204978121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df55e467ad20a0cd08e10d6c447177f88021735a54af168940f4548a0935e83a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:237e50f8a5f85c1b8bb5e54ccf6fc54cb7ca7cef794135e9c50fd64c812ec26d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:60f2a37f45af89cb5a543e58e191560ccc0da14b3ed1346578abc6873d702571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263707932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce213b690e983e6d1f65eec950595f8104e0b5a2a8c61823889ee8536220239`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:42:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:45 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:42:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 03:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:44:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:44:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:44:24 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:45:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:45:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:45:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:46:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341919f757e419f6142944f5ea95c19b61bf1ff648abdfff94ed8c99c0bfd52c`  
		Last Modified: Fri, 22 Apr 2022 03:55:07 GMT  
		Size: 1.2 MB (1191091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c8ef748e7b3e35f60511f8e8053ee76492c9a72a5afd00d55d351854556f`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 3.8 MB (3826746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b72761451ff916be9282f71adece9e357fc9710e86559b986d1f01583fd312`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3452459740e87b470a88f20122447689e1640a2b865eb50f2f4a866ad75d391`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2037c4fb46b3cec9022f679d45d7834d6c89ac325348efc7af3d5d92bcd7658`  
		Last Modified: Fri, 22 Apr 2022 03:55:22 GMT  
		Size: 106.4 MB (106381750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0221e7e4829eedc9594c53ce3492bccdc39ea2c1b77da83a10fdb689100c68`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c7fbeb7e1d7385b2109f0df086ca744db3d917acd012c123fa8edc585a2080`  
		Last Modified: Fri, 22 Apr 2022 03:55:46 GMT  
		Size: 98.8 MB (98754384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b30b9dcc84973150cb0c195863fd24646a6ba41a76b5f0b33c806b25f12281c`  
		Last Modified: Fri, 22 Apr 2022 03:55:33 GMT  
		Size: 268.9 KB (268885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8e6a2755512e3269961eabe5ea4b4f1aec52de907316bb4f8654466d684b8a`  
		Last Modified: Fri, 22 Apr 2022 03:55:32 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba940d517ddac55ea1379c9f2cff56d93e8aa91f44e1303dc4a4261a1ef6810`  
		Last Modified: Fri, 22 Apr 2022 03:55:36 GMT  
		Size: 22.9 MB (22859264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3dfe17f949018783272b299a2a59c3e69c11fca5672006cc9ebb9edf2188879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255944624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51069cd265c1e26edf301600ec514b3b806b206530fca8cf5b20fc19c589c66`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:31 GMT
ADD file:31ce105f73c45fb89d7f254c71800e97a4774b64b3dfbc215bfb05848493ecee in / 
# Fri, 22 Apr 2022 00:54:31 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:15:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:15:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:15:56 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:15:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:15:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 04:16:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:16:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:16:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:16:47 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:17:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:17:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:17:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:17:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b5ca5a85338a7c13939e3609f3880b846d36862cce227eecd4c12af971cde8f`  
		Last Modified: Fri, 22 Apr 2022 00:56:28 GMT  
		Size: 28.4 MB (28376083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb989802917175cdb271141f4e081fa8e989cb5709d21d8ac4153b95085d52c`  
		Last Modified: Fri, 22 Apr 2022 04:27:16 GMT  
		Size: 1.2 MB (1192171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283604da4b314ff67f723c5bf1ba2a93801b4ecd9373906ace9b9accc2ce21b6`  
		Last Modified: Fri, 22 Apr 2022 04:27:14 GMT  
		Size: 3.6 MB (3593959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497a2e9ad1660ac6f4277bb83eb2b381668a1df22804fcc63dc3c87b2fb0b5b`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac029af969ad05ee2f310912643789cec16385d1820a3f5d52a4fdb0f6e8a2`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b7f771226a391368da04fd28620f186d7424276903e001d9ccf0d49568f34`  
		Last Modified: Fri, 22 Apr 2022 04:27:30 GMT  
		Size: 104.1 MB (104118226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976669ac24504d62fd730fdc9ae05cc6fb959bbbc0dc1ad0f2f65954450b1681`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd1da39f9ae593499b9a4d3531127fd53836895c5cd5275c1e46e049e3c6b4d`  
		Last Modified: Fri, 22 Apr 2022 04:27:54 GMT  
		Size: 96.1 MB (96127137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a2e403ab0fabbcad25bddedfb2766fd50209e4c0e4af10d8aa5896d14a5260`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 268.8 KB (268831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfec5e8b47fa43a40b056c79b5047743be8d33a0356894a46708b23a5f805bd`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 2.1 KB (2129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2398acbb01abaf3b5232dfcdc0535d9e2d2d0a8c4d6b0d419803ee2c398f4a6`  
		Last Modified: Fri, 22 Apr 2022 04:27:44 GMT  
		Size: 22.3 MB (22263722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:237e50f8a5f85c1b8bb5e54ccf6fc54cb7ca7cef794135e9c50fd64c812ec26d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:60f2a37f45af89cb5a543e58e191560ccc0da14b3ed1346578abc6873d702571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263707932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce213b690e983e6d1f65eec950595f8104e0b5a2a8c61823889ee8536220239`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:42:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:45 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:42:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 03:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:44:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:44:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:44:24 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:45:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:45:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:45:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:46:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341919f757e419f6142944f5ea95c19b61bf1ff648abdfff94ed8c99c0bfd52c`  
		Last Modified: Fri, 22 Apr 2022 03:55:07 GMT  
		Size: 1.2 MB (1191091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c8ef748e7b3e35f60511f8e8053ee76492c9a72a5afd00d55d351854556f`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 3.8 MB (3826746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b72761451ff916be9282f71adece9e357fc9710e86559b986d1f01583fd312`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3452459740e87b470a88f20122447689e1640a2b865eb50f2f4a866ad75d391`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2037c4fb46b3cec9022f679d45d7834d6c89ac325348efc7af3d5d92bcd7658`  
		Last Modified: Fri, 22 Apr 2022 03:55:22 GMT  
		Size: 106.4 MB (106381750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0221e7e4829eedc9594c53ce3492bccdc39ea2c1b77da83a10fdb689100c68`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c7fbeb7e1d7385b2109f0df086ca744db3d917acd012c123fa8edc585a2080`  
		Last Modified: Fri, 22 Apr 2022 03:55:46 GMT  
		Size: 98.8 MB (98754384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b30b9dcc84973150cb0c195863fd24646a6ba41a76b5f0b33c806b25f12281c`  
		Last Modified: Fri, 22 Apr 2022 03:55:33 GMT  
		Size: 268.9 KB (268885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8e6a2755512e3269961eabe5ea4b4f1aec52de907316bb4f8654466d684b8a`  
		Last Modified: Fri, 22 Apr 2022 03:55:32 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba940d517ddac55ea1379c9f2cff56d93e8aa91f44e1303dc4a4261a1ef6810`  
		Last Modified: Fri, 22 Apr 2022 03:55:36 GMT  
		Size: 22.9 MB (22859264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3dfe17f949018783272b299a2a59c3e69c11fca5672006cc9ebb9edf2188879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255944624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51069cd265c1e26edf301600ec514b3b806b206530fca8cf5b20fc19c589c66`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:31 GMT
ADD file:31ce105f73c45fb89d7f254c71800e97a4774b64b3dfbc215bfb05848493ecee in / 
# Fri, 22 Apr 2022 00:54:31 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:15:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:15:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:15:56 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:15:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:15:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 04:16:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:16:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:16:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:16:47 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:17:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:17:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:17:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:17:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b5ca5a85338a7c13939e3609f3880b846d36862cce227eecd4c12af971cde8f`  
		Last Modified: Fri, 22 Apr 2022 00:56:28 GMT  
		Size: 28.4 MB (28376083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb989802917175cdb271141f4e081fa8e989cb5709d21d8ac4153b95085d52c`  
		Last Modified: Fri, 22 Apr 2022 04:27:16 GMT  
		Size: 1.2 MB (1192171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283604da4b314ff67f723c5bf1ba2a93801b4ecd9373906ace9b9accc2ce21b6`  
		Last Modified: Fri, 22 Apr 2022 04:27:14 GMT  
		Size: 3.6 MB (3593959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497a2e9ad1660ac6f4277bb83eb2b381668a1df22804fcc63dc3c87b2fb0b5b`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac029af969ad05ee2f310912643789cec16385d1820a3f5d52a4fdb0f6e8a2`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b7f771226a391368da04fd28620f186d7424276903e001d9ccf0d49568f34`  
		Last Modified: Fri, 22 Apr 2022 04:27:30 GMT  
		Size: 104.1 MB (104118226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976669ac24504d62fd730fdc9ae05cc6fb959bbbc0dc1ad0f2f65954450b1681`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd1da39f9ae593499b9a4d3531127fd53836895c5cd5275c1e46e049e3c6b4d`  
		Last Modified: Fri, 22 Apr 2022 04:27:54 GMT  
		Size: 96.1 MB (96127137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a2e403ab0fabbcad25bddedfb2766fd50209e4c0e4af10d8aa5896d14a5260`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 268.8 KB (268831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfec5e8b47fa43a40b056c79b5047743be8d33a0356894a46708b23a5f805bd`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 2.1 KB (2129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2398acbb01abaf3b5232dfcdc0535d9e2d2d0a8c4d6b0d419803ee2c398f4a6`  
		Last Modified: Fri, 22 Apr 2022 04:27:44 GMT  
		Size: 22.3 MB (22263722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:237e50f8a5f85c1b8bb5e54ccf6fc54cb7ca7cef794135e9c50fd64c812ec26d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:60f2a37f45af89cb5a543e58e191560ccc0da14b3ed1346578abc6873d702571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263707932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce213b690e983e6d1f65eec950595f8104e0b5a2a8c61823889ee8536220239`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:42:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:45 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:42:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 03:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:44:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:44:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:44:24 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:45:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:45:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:45:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:46:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341919f757e419f6142944f5ea95c19b61bf1ff648abdfff94ed8c99c0bfd52c`  
		Last Modified: Fri, 22 Apr 2022 03:55:07 GMT  
		Size: 1.2 MB (1191091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c8ef748e7b3e35f60511f8e8053ee76492c9a72a5afd00d55d351854556f`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 3.8 MB (3826746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b72761451ff916be9282f71adece9e357fc9710e86559b986d1f01583fd312`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3452459740e87b470a88f20122447689e1640a2b865eb50f2f4a866ad75d391`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2037c4fb46b3cec9022f679d45d7834d6c89ac325348efc7af3d5d92bcd7658`  
		Last Modified: Fri, 22 Apr 2022 03:55:22 GMT  
		Size: 106.4 MB (106381750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0221e7e4829eedc9594c53ce3492bccdc39ea2c1b77da83a10fdb689100c68`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c7fbeb7e1d7385b2109f0df086ca744db3d917acd012c123fa8edc585a2080`  
		Last Modified: Fri, 22 Apr 2022 03:55:46 GMT  
		Size: 98.8 MB (98754384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b30b9dcc84973150cb0c195863fd24646a6ba41a76b5f0b33c806b25f12281c`  
		Last Modified: Fri, 22 Apr 2022 03:55:33 GMT  
		Size: 268.9 KB (268885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8e6a2755512e3269961eabe5ea4b4f1aec52de907316bb4f8654466d684b8a`  
		Last Modified: Fri, 22 Apr 2022 03:55:32 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba940d517ddac55ea1379c9f2cff56d93e8aa91f44e1303dc4a4261a1ef6810`  
		Last Modified: Fri, 22 Apr 2022 03:55:36 GMT  
		Size: 22.9 MB (22859264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3dfe17f949018783272b299a2a59c3e69c11fca5672006cc9ebb9edf2188879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255944624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51069cd265c1e26edf301600ec514b3b806b206530fca8cf5b20fc19c589c66`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:31 GMT
ADD file:31ce105f73c45fb89d7f254c71800e97a4774b64b3dfbc215bfb05848493ecee in / 
# Fri, 22 Apr 2022 00:54:31 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:15:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:15:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:15:56 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:15:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:15:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 04:16:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:16:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:16:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:16:47 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:17:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:17:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:17:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:17:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b5ca5a85338a7c13939e3609f3880b846d36862cce227eecd4c12af971cde8f`  
		Last Modified: Fri, 22 Apr 2022 00:56:28 GMT  
		Size: 28.4 MB (28376083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb989802917175cdb271141f4e081fa8e989cb5709d21d8ac4153b95085d52c`  
		Last Modified: Fri, 22 Apr 2022 04:27:16 GMT  
		Size: 1.2 MB (1192171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283604da4b314ff67f723c5bf1ba2a93801b4ecd9373906ace9b9accc2ce21b6`  
		Last Modified: Fri, 22 Apr 2022 04:27:14 GMT  
		Size: 3.6 MB (3593959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497a2e9ad1660ac6f4277bb83eb2b381668a1df22804fcc63dc3c87b2fb0b5b`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac029af969ad05ee2f310912643789cec16385d1820a3f5d52a4fdb0f6e8a2`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b7f771226a391368da04fd28620f186d7424276903e001d9ccf0d49568f34`  
		Last Modified: Fri, 22 Apr 2022 04:27:30 GMT  
		Size: 104.1 MB (104118226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976669ac24504d62fd730fdc9ae05cc6fb959bbbc0dc1ad0f2f65954450b1681`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd1da39f9ae593499b9a4d3531127fd53836895c5cd5275c1e46e049e3c6b4d`  
		Last Modified: Fri, 22 Apr 2022 04:27:54 GMT  
		Size: 96.1 MB (96127137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a2e403ab0fabbcad25bddedfb2766fd50209e4c0e4af10d8aa5896d14a5260`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 268.8 KB (268831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfec5e8b47fa43a40b056c79b5047743be8d33a0356894a46708b23a5f805bd`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 2.1 KB (2129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2398acbb01abaf3b5232dfcdc0535d9e2d2d0a8c4d6b0d419803ee2c398f4a6`  
		Last Modified: Fri, 22 Apr 2022 04:27:44 GMT  
		Size: 22.3 MB (22263722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:1db1c9a3127ddf6ed5b86be14d78a7edbb025d06fa369c4a5731e606fa204483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f0db02e019e6a4b3934609861d6bd367d4d7ea1a5e549d9d4bf61b728a97d80b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141823212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15372d384c90753f1c0cffc69b1eab508dc0a8431ff96bb212b34f8218fd8b52`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:42:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:45 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:42:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 03:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:44:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:44:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:44:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341919f757e419f6142944f5ea95c19b61bf1ff648abdfff94ed8c99c0bfd52c`  
		Last Modified: Fri, 22 Apr 2022 03:55:07 GMT  
		Size: 1.2 MB (1191091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c8ef748e7b3e35f60511f8e8053ee76492c9a72a5afd00d55d351854556f`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 3.8 MB (3826746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b72761451ff916be9282f71adece9e357fc9710e86559b986d1f01583fd312`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3452459740e87b470a88f20122447689e1640a2b865eb50f2f4a866ad75d391`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2037c4fb46b3cec9022f679d45d7834d6c89ac325348efc7af3d5d92bcd7658`  
		Last Modified: Fri, 22 Apr 2022 03:55:22 GMT  
		Size: 106.4 MB (106381750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0221e7e4829eedc9594c53ce3492bccdc39ea2c1b77da83a10fdb689100c68`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4cb42493ab078a7338cef0a920df6a02850c0ae562532644ca0439f0f00aaf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137282805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afaa184a751f99ac19d1e1f7ccaba533e7422cb55071c3f48a0f3a601561c90`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:31 GMT
ADD file:31ce105f73c45fb89d7f254c71800e97a4774b64b3dfbc215bfb05848493ecee in / 
# Fri, 22 Apr 2022 00:54:31 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:15:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:15:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:15:56 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:15:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:15:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 04:16:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:16:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:16:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:16:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b5ca5a85338a7c13939e3609f3880b846d36862cce227eecd4c12af971cde8f`  
		Last Modified: Fri, 22 Apr 2022 00:56:28 GMT  
		Size: 28.4 MB (28376083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb989802917175cdb271141f4e081fa8e989cb5709d21d8ac4153b95085d52c`  
		Last Modified: Fri, 22 Apr 2022 04:27:16 GMT  
		Size: 1.2 MB (1192171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283604da4b314ff67f723c5bf1ba2a93801b4ecd9373906ace9b9accc2ce21b6`  
		Last Modified: Fri, 22 Apr 2022 04:27:14 GMT  
		Size: 3.6 MB (3593959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497a2e9ad1660ac6f4277bb83eb2b381668a1df22804fcc63dc3c87b2fb0b5b`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac029af969ad05ee2f310912643789cec16385d1820a3f5d52a4fdb0f6e8a2`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b7f771226a391368da04fd28620f186d7424276903e001d9ccf0d49568f34`  
		Last Modified: Fri, 22 Apr 2022 04:27:30 GMT  
		Size: 104.1 MB (104118226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976669ac24504d62fd730fdc9ae05cc6fb959bbbc0dc1ad0f2f65954450b1681`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:1db1c9a3127ddf6ed5b86be14d78a7edbb025d06fa369c4a5731e606fa204483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:f0db02e019e6a4b3934609861d6bd367d4d7ea1a5e549d9d4bf61b728a97d80b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141823212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15372d384c90753f1c0cffc69b1eab508dc0a8431ff96bb212b34f8218fd8b52`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:42:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:45 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:42:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 03:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:44:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:44:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:44:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341919f757e419f6142944f5ea95c19b61bf1ff648abdfff94ed8c99c0bfd52c`  
		Last Modified: Fri, 22 Apr 2022 03:55:07 GMT  
		Size: 1.2 MB (1191091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c8ef748e7b3e35f60511f8e8053ee76492c9a72a5afd00d55d351854556f`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 3.8 MB (3826746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b72761451ff916be9282f71adece9e357fc9710e86559b986d1f01583fd312`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3452459740e87b470a88f20122447689e1640a2b865eb50f2f4a866ad75d391`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2037c4fb46b3cec9022f679d45d7834d6c89ac325348efc7af3d5d92bcd7658`  
		Last Modified: Fri, 22 Apr 2022 03:55:22 GMT  
		Size: 106.4 MB (106381750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0221e7e4829eedc9594c53ce3492bccdc39ea2c1b77da83a10fdb689100c68`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4cb42493ab078a7338cef0a920df6a02850c0ae562532644ca0439f0f00aaf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137282805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afaa184a751f99ac19d1e1f7ccaba533e7422cb55071c3f48a0f3a601561c90`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:31 GMT
ADD file:31ce105f73c45fb89d7f254c71800e97a4774b64b3dfbc215bfb05848493ecee in / 
# Fri, 22 Apr 2022 00:54:31 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:15:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:15:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:15:56 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:15:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:15:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 04:16:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:16:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:16:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:16:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b5ca5a85338a7c13939e3609f3880b846d36862cce227eecd4c12af971cde8f`  
		Last Modified: Fri, 22 Apr 2022 00:56:28 GMT  
		Size: 28.4 MB (28376083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb989802917175cdb271141f4e081fa8e989cb5709d21d8ac4153b95085d52c`  
		Last Modified: Fri, 22 Apr 2022 04:27:16 GMT  
		Size: 1.2 MB (1192171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283604da4b314ff67f723c5bf1ba2a93801b4ecd9373906ace9b9accc2ce21b6`  
		Last Modified: Fri, 22 Apr 2022 04:27:14 GMT  
		Size: 3.6 MB (3593959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497a2e9ad1660ac6f4277bb83eb2b381668a1df22804fcc63dc3c87b2fb0b5b`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac029af969ad05ee2f310912643789cec16385d1820a3f5d52a4fdb0f6e8a2`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b7f771226a391368da04fd28620f186d7424276903e001d9ccf0d49568f34`  
		Last Modified: Fri, 22 Apr 2022 04:27:30 GMT  
		Size: 104.1 MB (104118226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976669ac24504d62fd730fdc9ae05cc6fb959bbbc0dc1ad0f2f65954450b1681`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
