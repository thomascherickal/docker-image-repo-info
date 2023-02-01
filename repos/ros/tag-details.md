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
$ docker pull ros@sha256:6383262372470ed7fc84c25775a690df8fa2cb569703e213626ec90023e0a8fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:d3ec5672bded3c6013dd0b0e84f9834c27086e0b183ae07c2068a72262707ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250919416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e94dae160a999c00d79942337d225c1c58699174b0ecbb07bd746a00ad4502`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:44:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:44:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587bd24e6d3bd17af2906318935c23cec69372158c04d4c0e2276c45f79a1f8`  
		Last Modified: Tue, 31 Jan 2023 20:11:55 GMT  
		Size: 73.3 MB (73334209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9589f9c9bae39b4cbb571d2095fa9e20972d7bedf34f56c71cb377b234aa7207`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06edf09eaea7b0d1b06ccd74d1c8af33e67656d5a32341b70f778dfa2fc7e17`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 2.4 KB (2432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20917058504694a3791959dd4dc87db6cd42cf6c632019971eea5c6474b355c2`  
		Last Modified: Tue, 31 Jan 2023 20:11:48 GMT  
		Size: 21.7 MB (21662318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b60414f3e133756c56fbac3320de3486b25b46d69e21e8698d729f04b3ae6450
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226787687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1201d81781763520c9ea20c63a732f455637558edca49b4f950104b80acb58a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:28:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:28:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 19:28:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adda8a81e2bf6c30215882e975243f6a170a540c87e8c7e3b1332fa416972c`  
		Last Modified: Wed, 01 Feb 2023 19:33:22 GMT  
		Size: 67.7 MB (67681881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec47ba32a1ca970ab95560eed5fda1d4f9f03b051a6e7339297c5d0ff2508bb`  
		Last Modified: Wed, 01 Feb 2023 19:33:15 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce524890c3bf979cb77c26228586bc1657bdd90214e8cceb0cadbf8808fad`  
		Last Modified: Wed, 01 Feb 2023 19:33:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bbba78bc114f5f6afc240ad05c8b56ce878ebf866200090d533ec6620ac128`  
		Last Modified: Wed, 01 Feb 2023 19:33:17 GMT  
		Size: 20.4 MB (20384862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:6383262372470ed7fc84c25775a690df8fa2cb569703e213626ec90023e0a8fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:d3ec5672bded3c6013dd0b0e84f9834c27086e0b183ae07c2068a72262707ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250919416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e94dae160a999c00d79942337d225c1c58699174b0ecbb07bd746a00ad4502`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:44:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:44:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587bd24e6d3bd17af2906318935c23cec69372158c04d4c0e2276c45f79a1f8`  
		Last Modified: Tue, 31 Jan 2023 20:11:55 GMT  
		Size: 73.3 MB (73334209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9589f9c9bae39b4cbb571d2095fa9e20972d7bedf34f56c71cb377b234aa7207`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06edf09eaea7b0d1b06ccd74d1c8af33e67656d5a32341b70f778dfa2fc7e17`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 2.4 KB (2432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20917058504694a3791959dd4dc87db6cd42cf6c632019971eea5c6474b355c2`  
		Last Modified: Tue, 31 Jan 2023 20:11:48 GMT  
		Size: 21.7 MB (21662318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b60414f3e133756c56fbac3320de3486b25b46d69e21e8698d729f04b3ae6450
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226787687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1201d81781763520c9ea20c63a732f455637558edca49b4f950104b80acb58a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:28:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:28:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 19:28:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adda8a81e2bf6c30215882e975243f6a170a540c87e8c7e3b1332fa416972c`  
		Last Modified: Wed, 01 Feb 2023 19:33:22 GMT  
		Size: 67.7 MB (67681881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec47ba32a1ca970ab95560eed5fda1d4f9f03b051a6e7339297c5d0ff2508bb`  
		Last Modified: Wed, 01 Feb 2023 19:33:15 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce524890c3bf979cb77c26228586bc1657bdd90214e8cceb0cadbf8808fad`  
		Last Modified: Wed, 01 Feb 2023 19:33:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bbba78bc114f5f6afc240ad05c8b56ce878ebf866200090d533ec6620ac128`  
		Last Modified: Wed, 01 Feb 2023 19:33:17 GMT  
		Size: 20.4 MB (20384862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:6383262372470ed7fc84c25775a690df8fa2cb569703e213626ec90023e0a8fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:d3ec5672bded3c6013dd0b0e84f9834c27086e0b183ae07c2068a72262707ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250919416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e94dae160a999c00d79942337d225c1c58699174b0ecbb07bd746a00ad4502`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:44:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:44:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587bd24e6d3bd17af2906318935c23cec69372158c04d4c0e2276c45f79a1f8`  
		Last Modified: Tue, 31 Jan 2023 20:11:55 GMT  
		Size: 73.3 MB (73334209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9589f9c9bae39b4cbb571d2095fa9e20972d7bedf34f56c71cb377b234aa7207`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06edf09eaea7b0d1b06ccd74d1c8af33e67656d5a32341b70f778dfa2fc7e17`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 2.4 KB (2432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20917058504694a3791959dd4dc87db6cd42cf6c632019971eea5c6474b355c2`  
		Last Modified: Tue, 31 Jan 2023 20:11:48 GMT  
		Size: 21.7 MB (21662318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b60414f3e133756c56fbac3320de3486b25b46d69e21e8698d729f04b3ae6450
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226787687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1201d81781763520c9ea20c63a732f455637558edca49b4f950104b80acb58a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:28:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:28:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 19:28:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adda8a81e2bf6c30215882e975243f6a170a540c87e8c7e3b1332fa416972c`  
		Last Modified: Wed, 01 Feb 2023 19:33:22 GMT  
		Size: 67.7 MB (67681881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec47ba32a1ca970ab95560eed5fda1d4f9f03b051a6e7339297c5d0ff2508bb`  
		Last Modified: Wed, 01 Feb 2023 19:33:15 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce524890c3bf979cb77c26228586bc1657bdd90214e8cceb0cadbf8808fad`  
		Last Modified: Wed, 01 Feb 2023 19:33:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bbba78bc114f5f6afc240ad05c8b56ce878ebf866200090d533ec6620ac128`  
		Last Modified: Wed, 01 Feb 2023 19:33:17 GMT  
		Size: 20.4 MB (20384862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:fc0710a38383b8ceabe029a87b522a975c13f24edf4859d6ffb0cf850aeeb440
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:2e19996a9381e3f98d5dd5681f4d4e4aab8e91764b6644537b226b82f7690d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155642679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d5695824b395ad401e6c40f70e642860f157682ac3881d682e1d3c06ee529c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d993a8d8ddaab94f857c7eeea4817209d7fa3f7f0028b82cd0810202243ba2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138440709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd69454231214178e8a50eb5ff795a92a57d203699ddd932390f3126d6bf8dc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:fc0710a38383b8ceabe029a87b522a975c13f24edf4859d6ffb0cf850aeeb440
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:2e19996a9381e3f98d5dd5681f4d4e4aab8e91764b6644537b226b82f7690d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155642679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d5695824b395ad401e6c40f70e642860f157682ac3881d682e1d3c06ee529c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d993a8d8ddaab94f857c7eeea4817209d7fa3f7f0028b82cd0810202243ba2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138440709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd69454231214178e8a50eb5ff795a92a57d203699ddd932390f3126d6bf8dc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:a2ae48ba0e805548aba576d7da33e5a7eb558af3fe828b1fb1c27732d6545dfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:ad49d5486d4f18c27bbd5a43e9c82eee8c870f15a629315884ee95be61542b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349019600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0fba0f6333ea96c55c3744fd2c72b3688f12d19912764dc502ddb242acde1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:44:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:44:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:45:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:45:18 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Jan 2023 19:45:18 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Jan 2023 19:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:57 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587bd24e6d3bd17af2906318935c23cec69372158c04d4c0e2276c45f79a1f8`  
		Last Modified: Tue, 31 Jan 2023 20:11:55 GMT  
		Size: 73.3 MB (73334209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9589f9c9bae39b4cbb571d2095fa9e20972d7bedf34f56c71cb377b234aa7207`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06edf09eaea7b0d1b06ccd74d1c8af33e67656d5a32341b70f778dfa2fc7e17`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 2.4 KB (2432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20917058504694a3791959dd4dc87db6cd42cf6c632019971eea5c6474b355c2`  
		Last Modified: Tue, 31 Jan 2023 20:11:48 GMT  
		Size: 21.7 MB (21662318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac032e991d1161d607d3070d68fdb31d6002bc5fbc2c7c2d8faca77f92376c56`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab4f85c71b205725d550cb61dab91e859f5c7d09b9360d91d5cf51267f6facd`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1fd5b2feb27aedbe99d898da57948097f733170938a3b3e78d19cf5c993086`  
		Last Modified: Tue, 31 Jan 2023 20:12:21 GMT  
		Size: 76.4 MB (76425495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b22a19e3db8effb381b6add35af1ed189384797e8fbf54248a4ecc847e06f5`  
		Last Modified: Tue, 31 Jan 2023 20:12:11 GMT  
		Size: 21.7 MB (21674062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1888223ca45436cd56eeea009914eb481039a545fa94fa0765ab08841a5310d4`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d613d38696ab3c45d22678d6ce5adb76673fad8cf53a536da222be4b80d05a56
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317605237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6a1bd93bbc2c863ca9d150026991c1bafe61190cf7b6500d84c66216dde544`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:28:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:28:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 19:28:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:29:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:29:05 GMT
ENV ROS1_DISTRO=noetic
# Wed, 01 Feb 2023 19:29:06 GMT
ENV ROS2_DISTRO=foxy
# Wed, 01 Feb 2023 19:29:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:39 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adda8a81e2bf6c30215882e975243f6a170a540c87e8c7e3b1332fa416972c`  
		Last Modified: Wed, 01 Feb 2023 19:33:22 GMT  
		Size: 67.7 MB (67681881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec47ba32a1ca970ab95560eed5fda1d4f9f03b051a6e7339297c5d0ff2508bb`  
		Last Modified: Wed, 01 Feb 2023 19:33:15 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce524890c3bf979cb77c26228586bc1657bdd90214e8cceb0cadbf8808fad`  
		Last Modified: Wed, 01 Feb 2023 19:33:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bbba78bc114f5f6afc240ad05c8b56ce878ebf866200090d533ec6620ac128`  
		Last Modified: Wed, 01 Feb 2023 19:33:17 GMT  
		Size: 20.4 MB (20384862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb743e68e44180e01c844a18c62383859bd90cfecbf975e6d3514143b1b5b16`  
		Last Modified: Wed, 01 Feb 2023 19:33:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb68ff40f9ab643b646bdd28ac51b25ae5d4b5172e71a895ce932cb09f11f936`  
		Last Modified: Wed, 01 Feb 2023 19:33:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc63d3f2a453d56ffc84be29895fc86fe9147f526e418b9a54c7e5d2102949a`  
		Last Modified: Wed, 01 Feb 2023 19:33:45 GMT  
		Size: 76.5 MB (76491984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e733adf20852512138fea893a09497b474e5e2eb66c426b7e20d8a6fabc148`  
		Last Modified: Wed, 01 Feb 2023 19:33:36 GMT  
		Size: 14.3 MB (14324939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131efeacb312fb02072a1ab567a7e9aba2cfb394a98d8d6e7dfdf5f76455d9dc`  
		Last Modified: Wed, 01 Feb 2023 19:33:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:a2ae48ba0e805548aba576d7da33e5a7eb558af3fe828b1fb1c27732d6545dfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:ad49d5486d4f18c27bbd5a43e9c82eee8c870f15a629315884ee95be61542b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349019600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0fba0f6333ea96c55c3744fd2c72b3688f12d19912764dc502ddb242acde1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:44:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:44:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:45:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:45:18 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Jan 2023 19:45:18 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Jan 2023 19:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:57 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587bd24e6d3bd17af2906318935c23cec69372158c04d4c0e2276c45f79a1f8`  
		Last Modified: Tue, 31 Jan 2023 20:11:55 GMT  
		Size: 73.3 MB (73334209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9589f9c9bae39b4cbb571d2095fa9e20972d7bedf34f56c71cb377b234aa7207`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06edf09eaea7b0d1b06ccd74d1c8af33e67656d5a32341b70f778dfa2fc7e17`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 2.4 KB (2432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20917058504694a3791959dd4dc87db6cd42cf6c632019971eea5c6474b355c2`  
		Last Modified: Tue, 31 Jan 2023 20:11:48 GMT  
		Size: 21.7 MB (21662318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac032e991d1161d607d3070d68fdb31d6002bc5fbc2c7c2d8faca77f92376c56`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab4f85c71b205725d550cb61dab91e859f5c7d09b9360d91d5cf51267f6facd`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1fd5b2feb27aedbe99d898da57948097f733170938a3b3e78d19cf5c993086`  
		Last Modified: Tue, 31 Jan 2023 20:12:21 GMT  
		Size: 76.4 MB (76425495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b22a19e3db8effb381b6add35af1ed189384797e8fbf54248a4ecc847e06f5`  
		Last Modified: Tue, 31 Jan 2023 20:12:11 GMT  
		Size: 21.7 MB (21674062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1888223ca45436cd56eeea009914eb481039a545fa94fa0765ab08841a5310d4`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d613d38696ab3c45d22678d6ce5adb76673fad8cf53a536da222be4b80d05a56
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317605237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6a1bd93bbc2c863ca9d150026991c1bafe61190cf7b6500d84c66216dde544`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:28:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:28:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 19:28:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:29:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:29:05 GMT
ENV ROS1_DISTRO=noetic
# Wed, 01 Feb 2023 19:29:06 GMT
ENV ROS2_DISTRO=foxy
# Wed, 01 Feb 2023 19:29:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:39 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adda8a81e2bf6c30215882e975243f6a170a540c87e8c7e3b1332fa416972c`  
		Last Modified: Wed, 01 Feb 2023 19:33:22 GMT  
		Size: 67.7 MB (67681881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec47ba32a1ca970ab95560eed5fda1d4f9f03b051a6e7339297c5d0ff2508bb`  
		Last Modified: Wed, 01 Feb 2023 19:33:15 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce524890c3bf979cb77c26228586bc1657bdd90214e8cceb0cadbf8808fad`  
		Last Modified: Wed, 01 Feb 2023 19:33:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bbba78bc114f5f6afc240ad05c8b56ce878ebf866200090d533ec6620ac128`  
		Last Modified: Wed, 01 Feb 2023 19:33:17 GMT  
		Size: 20.4 MB (20384862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb743e68e44180e01c844a18c62383859bd90cfecbf975e6d3514143b1b5b16`  
		Last Modified: Wed, 01 Feb 2023 19:33:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb68ff40f9ab643b646bdd28ac51b25ae5d4b5172e71a895ce932cb09f11f936`  
		Last Modified: Wed, 01 Feb 2023 19:33:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc63d3f2a453d56ffc84be29895fc86fe9147f526e418b9a54c7e5d2102949a`  
		Last Modified: Wed, 01 Feb 2023 19:33:45 GMT  
		Size: 76.5 MB (76491984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e733adf20852512138fea893a09497b474e5e2eb66c426b7e20d8a6fabc148`  
		Last Modified: Wed, 01 Feb 2023 19:33:36 GMT  
		Size: 14.3 MB (14324939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131efeacb312fb02072a1ab567a7e9aba2cfb394a98d8d6e7dfdf5f76455d9dc`  
		Last Modified: Wed, 01 Feb 2023 19:33:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:fbbb36620eaeeb971d56fecb2a71ad066ca0b9c519eb3e43ae58f6071ac72c2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:68d0f1cb0624c2becba5d4fe6d007c4fd99a992bbc2fa33dc59e4cfdf255db73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263047549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a7f3d015fbf1b8ac174c038036a4954d12efdeb3f47822b1eab0b754083db3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e72d8676099b02e2cb44e6b64527a0d3b14b553a5ecaddfd181894e9989e40a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255723220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8a481e72504797f6c869e56268b127621638c07f59926e505207f045ecd7b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:41:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:41:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:41:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab33b235b8e909f44d5bab92f0a562dbe4400d83e004c3a5d6a7e1495a16998`  
		Last Modified: Tue, 31 Jan 2023 20:03:23 GMT  
		Size: 95.5 MB (95474668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ae431bec95faaa56f23dcbffd9714107eaa97278bdfabd2f64badd3b37172`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 309.5 KB (309527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca51810f29d361529154ba111db38bf918bf4a3c26b098839e362109b9ce9d7`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7994b14cba6e2b9acf21cc975ac230564cfaf9bcc01b3dfbf14cf5823f28c8d1`  
		Last Modified: Tue, 31 Jan 2023 20:03:15 GMT  
		Size: 22.5 MB (22498082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:2af14d955401257123bf89556fbf2156cec4435e5845ffe6df04432fa8e2eece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:d06e5b50ffb8d883eb44c17f893214303835f42e8c9f1d6c0a54350cdc89d954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1091865055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09b412b9ee94fd11ccb29532fb33fbad61644354311b2952d5a0d09aeb18f58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:59:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbd8ef5d5445adbecacb5be10e51e890b60e50e6380376986e5a4ffd2fe34bf`  
		Last Modified: Tue, 31 Jan 2023 20:15:02 GMT  
		Size: 828.8 MB (828817506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9e13e4ea14f30f1e9fb2543ee949ccd31a9d6c29183754f003c97dda201868cf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043328466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad31d6015e0a4eb4e648cb4314c724e1a95e31581d63ba7a19d3336081c0097`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:41:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:41:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:41:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab33b235b8e909f44d5bab92f0a562dbe4400d83e004c3a5d6a7e1495a16998`  
		Last Modified: Tue, 31 Jan 2023 20:03:23 GMT  
		Size: 95.5 MB (95474668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ae431bec95faaa56f23dcbffd9714107eaa97278bdfabd2f64badd3b37172`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 309.5 KB (309527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca51810f29d361529154ba111db38bf918bf4a3c26b098839e362109b9ce9d7`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7994b14cba6e2b9acf21cc975ac230564cfaf9bcc01b3dfbf14cf5823f28c8d1`  
		Last Modified: Tue, 31 Jan 2023 20:03:15 GMT  
		Size: 22.5 MB (22498082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf90c9b732568d264fde2d68a7b492248eeb6acc35666f6158a2b1af063e214d`  
		Last Modified: Tue, 31 Jan 2023 20:04:59 GMT  
		Size: 787.6 MB (787605246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:2af14d955401257123bf89556fbf2156cec4435e5845ffe6df04432fa8e2eece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:d06e5b50ffb8d883eb44c17f893214303835f42e8c9f1d6c0a54350cdc89d954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1091865055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09b412b9ee94fd11ccb29532fb33fbad61644354311b2952d5a0d09aeb18f58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:59:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbd8ef5d5445adbecacb5be10e51e890b60e50e6380376986e5a4ffd2fe34bf`  
		Last Modified: Tue, 31 Jan 2023 20:15:02 GMT  
		Size: 828.8 MB (828817506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9e13e4ea14f30f1e9fb2543ee949ccd31a9d6c29183754f003c97dda201868cf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043328466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad31d6015e0a4eb4e648cb4314c724e1a95e31581d63ba7a19d3336081c0097`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:41:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:41:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:41:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab33b235b8e909f44d5bab92f0a562dbe4400d83e004c3a5d6a7e1495a16998`  
		Last Modified: Tue, 31 Jan 2023 20:03:23 GMT  
		Size: 95.5 MB (95474668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ae431bec95faaa56f23dcbffd9714107eaa97278bdfabd2f64badd3b37172`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 309.5 KB (309527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca51810f29d361529154ba111db38bf918bf4a3c26b098839e362109b9ce9d7`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7994b14cba6e2b9acf21cc975ac230564cfaf9bcc01b3dfbf14cf5823f28c8d1`  
		Last Modified: Tue, 31 Jan 2023 20:03:15 GMT  
		Size: 22.5 MB (22498082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf90c9b732568d264fde2d68a7b492248eeb6acc35666f6158a2b1af063e214d`  
		Last Modified: Tue, 31 Jan 2023 20:04:59 GMT  
		Size: 787.6 MB (787605246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:fbbb36620eaeeb971d56fecb2a71ad066ca0b9c519eb3e43ae58f6071ac72c2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:68d0f1cb0624c2becba5d4fe6d007c4fd99a992bbc2fa33dc59e4cfdf255db73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263047549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a7f3d015fbf1b8ac174c038036a4954d12efdeb3f47822b1eab0b754083db3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e72d8676099b02e2cb44e6b64527a0d3b14b553a5ecaddfd181894e9989e40a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255723220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8a481e72504797f6c869e56268b127621638c07f59926e505207f045ecd7b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:41:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:41:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:41:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab33b235b8e909f44d5bab92f0a562dbe4400d83e004c3a5d6a7e1495a16998`  
		Last Modified: Tue, 31 Jan 2023 20:03:23 GMT  
		Size: 95.5 MB (95474668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ae431bec95faaa56f23dcbffd9714107eaa97278bdfabd2f64badd3b37172`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 309.5 KB (309527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca51810f29d361529154ba111db38bf918bf4a3c26b098839e362109b9ce9d7`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7994b14cba6e2b9acf21cc975ac230564cfaf9bcc01b3dfbf14cf5823f28c8d1`  
		Last Modified: Tue, 31 Jan 2023 20:03:15 GMT  
		Size: 22.5 MB (22498082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:fbbb36620eaeeb971d56fecb2a71ad066ca0b9c519eb3e43ae58f6071ac72c2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:68d0f1cb0624c2becba5d4fe6d007c4fd99a992bbc2fa33dc59e4cfdf255db73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263047549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a7f3d015fbf1b8ac174c038036a4954d12efdeb3f47822b1eab0b754083db3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e72d8676099b02e2cb44e6b64527a0d3b14b553a5ecaddfd181894e9989e40a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255723220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8a481e72504797f6c869e56268b127621638c07f59926e505207f045ecd7b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:41:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:41:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:41:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab33b235b8e909f44d5bab92f0a562dbe4400d83e004c3a5d6a7e1495a16998`  
		Last Modified: Tue, 31 Jan 2023 20:03:23 GMT  
		Size: 95.5 MB (95474668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ae431bec95faaa56f23dcbffd9714107eaa97278bdfabd2f64badd3b37172`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 309.5 KB (309527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca51810f29d361529154ba111db38bf918bf4a3c26b098839e362109b9ce9d7`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7994b14cba6e2b9acf21cc975ac230564cfaf9bcc01b3dfbf14cf5823f28c8d1`  
		Last Modified: Tue, 31 Jan 2023 20:03:15 GMT  
		Size: 22.5 MB (22498082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:b69e30779bca5958137a2fe63d3207d2b497d50038d7c5f5196a28214bfa0638
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ba8e85191b19e61f3c24f06a4baffd5bba4849b11a6021d294f88d4adbd2ebf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141778404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c00534496f6b5f76be21cd9803c18fb05ae946c67b959f4121c787956f88c55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c92912c2fc0b0799cd512de2ce82a80d233d66d4ffe1e8448f5104435db52fc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137438521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb767f468bcb53677f7f6da302811c6a39008d34066a96aec14ecaf7ef94776`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:b69e30779bca5958137a2fe63d3207d2b497d50038d7c5f5196a28214bfa0638
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:ba8e85191b19e61f3c24f06a4baffd5bba4849b11a6021d294f88d4adbd2ebf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141778404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c00534496f6b5f76be21cd9803c18fb05ae946c67b959f4121c787956f88c55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c92912c2fc0b0799cd512de2ce82a80d233d66d4ffe1e8448f5104435db52fc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137438521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb767f468bcb53677f7f6da302811c6a39008d34066a96aec14ecaf7ef94776`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:fbbb36620eaeeb971d56fecb2a71ad066ca0b9c519eb3e43ae58f6071ac72c2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:68d0f1cb0624c2becba5d4fe6d007c4fd99a992bbc2fa33dc59e4cfdf255db73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263047549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a7f3d015fbf1b8ac174c038036a4954d12efdeb3f47822b1eab0b754083db3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e72d8676099b02e2cb44e6b64527a0d3b14b553a5ecaddfd181894e9989e40a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255723220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8a481e72504797f6c869e56268b127621638c07f59926e505207f045ecd7b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:40:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:40:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:40:52 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:41:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:41:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:41:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af9e3000c81c2c6651161f46b5442c5c2f5b80a337ee45fc7822bed0887dc1`  
		Last Modified: Tue, 31 Jan 2023 20:03:03 GMT  
		Size: 104.1 MB (104078403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85471c723639473dc46c36c98880aebcce4bffc35ca94ed93d6cb8807938d6b6`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab33b235b8e909f44d5bab92f0a562dbe4400d83e004c3a5d6a7e1495a16998`  
		Last Modified: Tue, 31 Jan 2023 20:03:23 GMT  
		Size: 95.5 MB (95474668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ae431bec95faaa56f23dcbffd9714107eaa97278bdfabd2f64badd3b37172`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 309.5 KB (309527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca51810f29d361529154ba111db38bf918bf4a3c26b098839e362109b9ce9d7`  
		Last Modified: Tue, 31 Jan 2023 20:03:12 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7994b14cba6e2b9acf21cc975ac230564cfaf9bcc01b3dfbf14cf5823f28c8d1`  
		Last Modified: Tue, 31 Jan 2023 20:03:15 GMT  
		Size: 22.5 MB (22498082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:a423722cd718ebba9f6e931542d141b9336c609aca62136237147229567a2e65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:fb723744019f7fd23ecdf827d98f438840ed49bc04be33b84b9394c90c2c20cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437545037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3373bdb88182d13d88b174fec2db62c13515f5c07f9e9f99accde09d5e431d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c2bb574e034735f687dad3f78b30822b56f93ecc67099939469a79b8732190ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62a82935fb270cc1459cc69df1e3ffba90f30fd177f408c00150af724fa04b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbc4321812febb57cf26ee000188f548fa7f7896777a8de6532b5c954547e210
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412186398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f22525eac142b3219ca19244a21332c32edb778f702c2452226dd59965f9ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:c92bb6c989766bdc662b06a585e92f9bdaf20ec9088ec4290608588d42b28795
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:155398f60d3545bf238df052694e0363351909a847253ad98b335e0be5bc05d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742910719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:571b703f60b87fbe671af7614e6207566ec9c335d5f14d152333520cf3d55141`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:29:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9917cc891f3cc9fdcdca37d543e93aed743c1ff129b90eb18a423d7616e00c98`  
		Last Modified: Tue, 31 Jan 2023 20:08:32 GMT  
		Size: 305.4 MB (305365682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6ccfe204a6937e51ff88a1ab704577df8c1ff696a78e1b7fadefba632deae5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.1 MB (646063988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6a2633dcc2a91e278b960c1f3415c4326c51f4d0bb0b57b9352728568eef26a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd995ea923540db146755006760f9c6b275fae4455a4480824e7e90d6938e6a`  
		Last Modified: Tue, 31 Jan 2023 18:50:50 GMT  
		Size: 260.0 MB (260035585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9cba952bb66ba977a6e029880071a768d0b959c7ad2459b11e851902bff6d20e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.9 MB (703874129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa24332235bb63b1679306a62236142ca38a5ba62f01592f6d6d4ac2665a7ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7470adb3e62da1a8211f43ab68a221e0a289c9066912bb771297f4d5bb9c18da`  
		Last Modified: Tue, 31 Jan 2023 19:59:09 GMT  
		Size: 291.7 MB (291687731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:c92bb6c989766bdc662b06a585e92f9bdaf20ec9088ec4290608588d42b28795
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:155398f60d3545bf238df052694e0363351909a847253ad98b335e0be5bc05d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742910719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:571b703f60b87fbe671af7614e6207566ec9c335d5f14d152333520cf3d55141`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:29:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9917cc891f3cc9fdcdca37d543e93aed743c1ff129b90eb18a423d7616e00c98`  
		Last Modified: Tue, 31 Jan 2023 20:08:32 GMT  
		Size: 305.4 MB (305365682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6ccfe204a6937e51ff88a1ab704577df8c1ff696a78e1b7fadefba632deae5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.1 MB (646063988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6a2633dcc2a91e278b960c1f3415c4326c51f4d0bb0b57b9352728568eef26a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd995ea923540db146755006760f9c6b275fae4455a4480824e7e90d6938e6a`  
		Last Modified: Tue, 31 Jan 2023 18:50:50 GMT  
		Size: 260.0 MB (260035585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9cba952bb66ba977a6e029880071a768d0b959c7ad2459b11e851902bff6d20e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.9 MB (703874129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa24332235bb63b1679306a62236142ca38a5ba62f01592f6d6d4ac2665a7ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7470adb3e62da1a8211f43ab68a221e0a289c9066912bb771297f4d5bb9c18da`  
		Last Modified: Tue, 31 Jan 2023 19:59:09 GMT  
		Size: 291.7 MB (291687731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:9d78261b2aa127bc2573b61083b17162aaf3259f481b6fdd0301e3df99bd9d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:def62d1d38f09f81944eeb65ab71249580fe06b1ad4ef4a7228bcd27356d97df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448631605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668e2378e6271c7e4afdf3bcf7e7bef710ce191814ecff183121bae639660d55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:23:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b57f61ea25b8599ac645fc91fead462fb8a3b1a9288945f41195acf2db6a8c`  
		Last Modified: Tue, 31 Jan 2023 20:07:36 GMT  
		Size: 11.1 MB (11086568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:ed0a2283cfecd74266313eb3d6e3e9ed866d08e0662349693d5a864e51409211
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396151607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6bb107ccbd29f20a988cd58515f9afb873ccb64128ff4a7f7115ea13fd1859`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:26:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8360dfdcedceb583968fec82225dfdd9965d2db51a67247ff507977a1eab05f4`  
		Last Modified: Tue, 31 Jan 2023 18:49:55 GMT  
		Size: 10.1 MB (10123204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c7beeae06e92284331602616a8c6d8691909f7fd7abf614719b6803cdc954286
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422927478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684bf7ed7bb2d5abc2e931466b2b2911f3c8971927a86da89fa44cd97724e273`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fad0e68d9bbbd6deed548f188861d15fecdb6233f42ef0733b4ed9dc127b23c`  
		Last Modified: Tue, 31 Jan 2023 19:58:22 GMT  
		Size: 10.7 MB (10741080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:9d78261b2aa127bc2573b61083b17162aaf3259f481b6fdd0301e3df99bd9d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:def62d1d38f09f81944eeb65ab71249580fe06b1ad4ef4a7228bcd27356d97df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448631605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668e2378e6271c7e4afdf3bcf7e7bef710ce191814ecff183121bae639660d55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:23:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b57f61ea25b8599ac645fc91fead462fb8a3b1a9288945f41195acf2db6a8c`  
		Last Modified: Tue, 31 Jan 2023 20:07:36 GMT  
		Size: 11.1 MB (11086568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ed0a2283cfecd74266313eb3d6e3e9ed866d08e0662349693d5a864e51409211
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396151607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6bb107ccbd29f20a988cd58515f9afb873ccb64128ff4a7f7115ea13fd1859`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:26:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8360dfdcedceb583968fec82225dfdd9965d2db51a67247ff507977a1eab05f4`  
		Last Modified: Tue, 31 Jan 2023 18:49:55 GMT  
		Size: 10.1 MB (10123204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c7beeae06e92284331602616a8c6d8691909f7fd7abf614719b6803cdc954286
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422927478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684bf7ed7bb2d5abc2e931466b2b2911f3c8971927a86da89fa44cd97724e273`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fad0e68d9bbbd6deed548f188861d15fecdb6233f42ef0733b4ed9dc127b23c`  
		Last Modified: Tue, 31 Jan 2023 19:58:22 GMT  
		Size: 10.7 MB (10741080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:a423722cd718ebba9f6e931542d141b9336c609aca62136237147229567a2e65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:fb723744019f7fd23ecdf827d98f438840ed49bc04be33b84b9394c90c2c20cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437545037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3373bdb88182d13d88b174fec2db62c13515f5c07f9e9f99accde09d5e431d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:c2bb574e034735f687dad3f78b30822b56f93ecc67099939469a79b8732190ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62a82935fb270cc1459cc69df1e3ffba90f30fd177f408c00150af724fa04b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbc4321812febb57cf26ee000188f548fa7f7896777a8de6532b5c954547e210
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412186398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f22525eac142b3219ca19244a21332c32edb778f702c2452226dd59965f9ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:a423722cd718ebba9f6e931542d141b9336c609aca62136237147229567a2e65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:fb723744019f7fd23ecdf827d98f438840ed49bc04be33b84b9394c90c2c20cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437545037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3373bdb88182d13d88b174fec2db62c13515f5c07f9e9f99accde09d5e431d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c2bb574e034735f687dad3f78b30822b56f93ecc67099939469a79b8732190ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62a82935fb270cc1459cc69df1e3ffba90f30fd177f408c00150af724fa04b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbc4321812febb57cf26ee000188f548fa7f7896777a8de6532b5c954547e210
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412186398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f22525eac142b3219ca19244a21332c32edb778f702c2452226dd59965f9ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:13:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:13:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ff7870888fd7c2689a34ee0c08e62fa57bee0e5d98b52bebc5cf1dcda394a`  
		Last Modified: Tue, 31 Jan 2023 19:58:06 GMT  
		Size: 63.1 MB (63096000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc824988bb5fd5c68aca3c7d45ecd9cd00ed0e24d258fa00bc730849bed3ba4`  
		Last Modified: Tue, 31 Jan 2023 19:58:00 GMT  
		Size: 296.5 KB (296508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba479b0958ccd24153a47d4c5c9b9f25672e1388ad2b3449a3fbe8b3db1d8cc`  
		Last Modified: Tue, 31 Jan 2023 19:58:10 GMT  
		Size: 67.2 MB (67235785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:72997e34a5f6bc7f77da3756a4425eb4f7eca7ea2235f15799ea51a6eea02096
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:08215074eb025245f161f24ac6b005d497f37610cee0ec6610d0b3ee00207440
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291981629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd115d7130c39cb48762a7f348cbe8184a8b07993a9ea8de6e65a906090c448`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:74ab80b220e0f926f837786178e2f503267655eb4dd06de9019ac37dfcaef2d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266247093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18573c3a39388f3530ab15aeab3aa438867e3b371358444348a971250b3566fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:17b9997cdcac1ce4d094349795dab0a3e9ff134067d23e3292df3c461a405e71
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281558105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7508a6376c30f6d3969cc943174d45883d5a83016c38fb2eaa3eaefa54172443`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:72997e34a5f6bc7f77da3756a4425eb4f7eca7ea2235f15799ea51a6eea02096
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:08215074eb025245f161f24ac6b005d497f37610cee0ec6610d0b3ee00207440
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291981629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd115d7130c39cb48762a7f348cbe8184a8b07993a9ea8de6e65a906090c448`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:74ab80b220e0f926f837786178e2f503267655eb4dd06de9019ac37dfcaef2d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266247093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18573c3a39388f3530ab15aeab3aa438867e3b371358444348a971250b3566fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:17b9997cdcac1ce4d094349795dab0a3e9ff134067d23e3292df3c461a405e71
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281558105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7508a6376c30f6d3969cc943174d45883d5a83016c38fb2eaa3eaefa54172443`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:08:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:09:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:09:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:09:02 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:12:28 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:12:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:12:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07ee3e3960c32779378327e6f45b0cd530d673aaafbc3bb02ebf81f340f231e`  
		Last Modified: Tue, 31 Jan 2023 19:57:20 GMT  
		Size: 819.9 KB (819907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ad94c7976c1f0f92300e8bf04d61b97cdbd29d3abceaeb552e6521cbed456`  
		Last Modified: Tue, 31 Jan 2023 19:57:19 GMT  
		Size: 4.5 MB (4462834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efd42af4fc7886de98ff96d096d4ed7b9405745d9c8906d5653f976ae45d47`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab8439c1d060a597f2d5eeff25fd2eae59f3e64978304b242eb00a01cbda2`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402da9bc8f48c19c5a9c90957224b0897438f973cb1974d5c3cb2e0cf2a9152`  
		Last Modified: Tue, 31 Jan 2023 19:57:51 GMT  
		Size: 252.5 MB (252537988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6d1f86048a05a76b199644c17bad44b57ff7c17d5c2797c33a2f0f81cbd9a`  
		Last Modified: Tue, 31 Jan 2023 19:57:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:3e95165652987da802b4b70b24a5e68da5381de86a3ee5b5b73a9566c7b0abdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:093dfb05e09d5198362a3f1a69e887c0873c1311bf065fb33816fdc73989743c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343190067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9a9bf50e26daeaaee850bb232ed2a4376df3419ca4ef731987d5afbb0fb13a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ea8683583e242df0297c9b3921ae5cd4a67ce45139a231f5cd59186407b2af91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289276893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5790bb8151cfbe7c196aa9550d6d53fdfb33e9fb064738db698e49a610ff4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87fe54a6ded5be95e141e9a11f8bd23cc13088e3e01244cf46c98c1e807e72f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d3994a361be4ea5cbd11474d8877364831d3bedc228ad3ac2a76e8d7ce7eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:e12ad727a147824b8ede3bf0ae386c70fc0bd193b25d76acda251522f886debe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:5d9b84d1a80e0ca534ecca1c4dc021d36b2e58751bd46170f680bc439e1971e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835163354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7880d8ce1763209068646879aaee1b4db773a15f27eff4d6664d0e158c436baa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:42:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260fd7b5f44fab914eb69836104a2061145dba37429bac6110dda9950d899f4f`  
		Last Modified: Tue, 31 Jan 2023 20:11:05 GMT  
		Size: 492.0 MB (491973287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:37bc559aada21cfd1d8b060bb11a24b3d94135ba47bc6c066b4645d530d71496
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726201215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd2d8538af8a938c1cfc91632881a2408e588942556f8064dd7e740d360e0db`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f9738fde0a45a28f4838057458875da1a2ad3ed696d9c2ae6af7682f2a59c`  
		Last Modified: Wed, 01 Feb 2023 18:56:45 GMT  
		Size: 436.9 MB (436924322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0402ed089f38a4eae34423f94e53252d5f3f51cf27e2465451c5f326e03bc36e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785410796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006416c28f3c81d37b417b37bc18721624252ff30af46b7472d95da9db3d9eb9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:26:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96eb9797dd9598d9388204f1ac972b580efac99be5eeb571a5c8f7cdee8bc4`  
		Last Modified: Wed, 01 Feb 2023 19:32:41 GMT  
		Size: 462.6 MB (462563297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:cfb2234b12bb76cbadb74687c0718438804735a60435ceacc499a6cb0be4b5b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:2bbf63fcb0a536fe0321fd0d52e31ae875519aa7c26cf0c4b24fe3b51016dacc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.3 MB (951257321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc241f6d9ea5863f7dc4fd6368d9216be675f4bc3738ac1ceeab7d5949504172`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:54 GMT
ADD file:4bf66d4081da52e8b692fcff96aad84d3e68bda4f62e870e8f4803153c70e24c in / 
# Wed, 11 Jan 2023 02:34:55 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:21:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:21:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 17:21:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 17:21:40 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 17:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:22:58 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 17:22:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 17:22:59 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:23:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:23:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 Jan 2023 17:24:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:27:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac7f2e1c758675427623d0da4faa88b336c62466c15a98af61efd3f015282f2f`  
		Last Modified: Wed, 11 Jan 2023 02:39:26 GMT  
		Size: 50.4 MB (50448910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed05e22e781556eb3057b10b25e54b8161dad941a5286d7328b50bba2f679b`  
		Last Modified: Wed, 11 Jan 2023 17:29:02 GMT  
		Size: 10.9 MB (10897026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6546cbd4873db6f5862f15a5a02564919836e584e6d1ea33023aa1dd4cdf72f6`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7289081c9d2531b3beccb982cbaefbe997da2cc44528869692cca6bf31ea17`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03333b8952a2f078f37ed6511a22271194ed1d51350d49a57fea72622f4ebac9`  
		Last Modified: Wed, 11 Jan 2023 17:29:33 GMT  
		Size: 239.3 MB (239251419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af920c4677ebb81ba3c51dfea10714e63a1b5819f57dc6c67908a8ad8eccfc`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e754f5425abb4e7c144f985ae140d29c7317db661da308682c81f1a76f3247`  
		Last Modified: Wed, 11 Jan 2023 17:29:51 GMT  
		Size: 86.6 MB (86602948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d11cda2ebbd36d930349879770ec5693b9d903dd36eac0bc8b860aceef9a52`  
		Last Modified: Wed, 11 Jan 2023 17:29:39 GMT  
		Size: 335.5 KB (335525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e3a8dedc38d35e970ad02976d8fd342416f69d45aad155d607eb0f983bd86f`  
		Last Modified: Wed, 11 Jan 2023 17:29:49 GMT  
		Size: 76.0 MB (75978213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d024f555c23852eec4a9199341ab63f70668805556a7224b888ef03b3696eba1`  
		Last Modified: Wed, 11 Jan 2023 17:31:20 GMT  
		Size: 487.7 MB (487740866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bcac92ef066c85908f8a9fece35dab503c63f5b3df4bd5f70caefe2a9c868287
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.1 MB (868065908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861356b5105a3440f60a6cca1d4e1f230d2351ffdc079879d5f6cf1792a3b1ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:43 GMT
ADD file:6b2b58305052bb953886c976022efeb324ef33bc6e55f9e15915e98490bd8fcb in / 
# Wed, 11 Jan 2023 02:57:43 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:52:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:52:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 13:52:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 13:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:53:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 13:53:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 13:53:46 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:54:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:54:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 Jan 2023 13:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:59:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15639959ffec1b29b8f88b1e1db3ca0574ca52ee28fd8f3ac6d2cbb1c85fb209`  
		Last Modified: Wed, 11 Jan 2023 03:01:37 GMT  
		Size: 49.2 MB (49233802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426afb0be41a462ca64e39ae6a74ed19ce54db5cd4d8fc00b5094120e8fa8f2`  
		Last Modified: Wed, 11 Jan 2023 14:00:58 GMT  
		Size: 10.9 MB (10902625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71036bab13158db91bd98501b67328211754dad8cac28846bf4aa4ecbde4d658`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e7410b12ea7be4c80024e40f3adcd15efb8dd2b0b24abe4227c4f21cfa894b`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f2c8b362ea16751add95c3717f39e7f30cf2649c3affcc6ae88a08aeab9a5b`  
		Last Modified: Wed, 11 Jan 2023 14:01:21 GMT  
		Size: 184.4 MB (184440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f46ce4b267a4a43fa1378cdd5ec96948d2840335e4ca90ab3100c67516d4c6`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc73cadcad0750f2ced4b8a64f684d077dbc86dfcb490e0705f01e359820dc26`  
		Last Modified: Wed, 11 Jan 2023 14:01:36 GMT  
		Size: 84.4 MB (84392048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2f8d1d96d181162c436accd0a6a33bc249984e8e5ad2fc5476f0e4dd056bcc`  
		Last Modified: Wed, 11 Jan 2023 14:01:28 GMT  
		Size: 335.5 KB (335525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7756844afb4448a1b4c4ef76967534312274fc784844e8f40aa841618908afb6`  
		Last Modified: Wed, 11 Jan 2023 14:01:35 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949de7bcc3313de93f2e1915d5d566944cd640f29c93c1112baa9f8e6cab0cb4`  
		Last Modified: Wed, 11 Jan 2023 14:02:42 GMT  
		Size: 464.7 MB (464668390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:e12ad727a147824b8ede3bf0ae386c70fc0bd193b25d76acda251522f886debe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:5d9b84d1a80e0ca534ecca1c4dc021d36b2e58751bd46170f680bc439e1971e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835163354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7880d8ce1763209068646879aaee1b4db773a15f27eff4d6664d0e158c436baa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:42:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260fd7b5f44fab914eb69836104a2061145dba37429bac6110dda9950d899f4f`  
		Last Modified: Tue, 31 Jan 2023 20:11:05 GMT  
		Size: 492.0 MB (491973287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:37bc559aada21cfd1d8b060bb11a24b3d94135ba47bc6c066b4645d530d71496
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726201215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd2d8538af8a938c1cfc91632881a2408e588942556f8064dd7e740d360e0db`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f9738fde0a45a28f4838057458875da1a2ad3ed696d9c2ae6af7682f2a59c`  
		Last Modified: Wed, 01 Feb 2023 18:56:45 GMT  
		Size: 436.9 MB (436924322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0402ed089f38a4eae34423f94e53252d5f3f51cf27e2465451c5f326e03bc36e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785410796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006416c28f3c81d37b417b37bc18721624252ff30af46b7472d95da9db3d9eb9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:26:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96eb9797dd9598d9388204f1ac972b580efac99be5eeb571a5c8f7cdee8bc4`  
		Last Modified: Wed, 01 Feb 2023 19:32:41 GMT  
		Size: 462.6 MB (462563297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:c8cd309e369694d9a472e6669d5860f82ed91e2929da73f809740c323bbb9975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:e7b73f0751dfaf6f249acf7942ba501f8211b94f9e87e67d26a86374d9955f75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359051603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d373974956dd933f9b21ff58168da8fc15cf52a8c6622919719ad011dd850fb4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:36:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22cf93466a9664a9f256c543ada4cb318001c3cf0e631a6e27ed07729dd6355`  
		Last Modified: Tue, 31 Jan 2023 20:09:44 GMT  
		Size: 15.9 MB (15861536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:212560e1cfe592fde12b0668d26a53663f13dedb03e9cbba7662bee9a39fccd9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303343639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba2dedd13d8892bbee3062acd62fb3daafe99715fd9ef3ab3b47ef036e4b47e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f465c6d63ea021516db6106f057d26b8f3ec5b3ea6b8923d4ea13332b4388fd`  
		Last Modified: Wed, 01 Feb 2023 18:55:21 GMT  
		Size: 14.1 MB (14066746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d60eb59c5d99b1d4540311c0096a3f7d82c7b47db6251ade8d926ef82180e0f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338304671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03d47df4b22b25bedb4a11e28c7363ace9cb739f111eb0c7c4b327566dcd67f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:19:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980521b22f06972d2449b80e28733c86c079e2c641b54af5272449178586a1c4`  
		Last Modified: Wed, 01 Feb 2023 19:31:42 GMT  
		Size: 15.5 MB (15457172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:c5c224b4af877028a8ad9fe48c3b3de0e6363f4bb5c594937cca3ea980089ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:7c6ad938ed1a8d945c916fa17e2401d669343f06203728a33bbde63267191e78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484671613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fa5fcc2c83f80147e1bf07614863fe9981db5761b40948ed57aff829aff0150`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:54 GMT
ADD file:4bf66d4081da52e8b692fcff96aad84d3e68bda4f62e870e8f4803153c70e24c in / 
# Wed, 11 Jan 2023 02:34:55 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:21:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:21:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 17:21:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 17:21:40 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 17:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:22:58 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 17:22:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 17:22:59 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:23:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:23:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 Jan 2023 17:24:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:24:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac7f2e1c758675427623d0da4faa88b336c62466c15a98af61efd3f015282f2f`  
		Last Modified: Wed, 11 Jan 2023 02:39:26 GMT  
		Size: 50.4 MB (50448910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed05e22e781556eb3057b10b25e54b8161dad941a5286d7328b50bba2f679b`  
		Last Modified: Wed, 11 Jan 2023 17:29:02 GMT  
		Size: 10.9 MB (10897026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6546cbd4873db6f5862f15a5a02564919836e584e6d1ea33023aa1dd4cdf72f6`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7289081c9d2531b3beccb982cbaefbe997da2cc44528869692cca6bf31ea17`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03333b8952a2f078f37ed6511a22271194ed1d51350d49a57fea72622f4ebac9`  
		Last Modified: Wed, 11 Jan 2023 17:29:33 GMT  
		Size: 239.3 MB (239251419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af920c4677ebb81ba3c51dfea10714e63a1b5819f57dc6c67908a8ad8eccfc`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e754f5425abb4e7c144f985ae140d29c7317db661da308682c81f1a76f3247`  
		Last Modified: Wed, 11 Jan 2023 17:29:51 GMT  
		Size: 86.6 MB (86602948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d11cda2ebbd36d930349879770ec5693b9d903dd36eac0bc8b860aceef9a52`  
		Last Modified: Wed, 11 Jan 2023 17:29:39 GMT  
		Size: 335.5 KB (335525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e3a8dedc38d35e970ad02976d8fd342416f69d45aad155d607eb0f983bd86f`  
		Last Modified: Wed, 11 Jan 2023 17:29:49 GMT  
		Size: 76.0 MB (75978213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2046db598f78b0b5481114a30bbae0d1ec816bca4f7a615175d56a35d0c9a922`  
		Last Modified: Wed, 11 Jan 2023 17:30:00 GMT  
		Size: 21.2 MB (21155158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed477a6be40e207acabea7d63edf972e40423376f47ad8ab2f7c2155af2ef8b3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424216536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ba788c7fd4f8a2b2e64980a0826988a1226da2e9341ebfe57e36fc94c03c37`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:43 GMT
ADD file:6b2b58305052bb953886c976022efeb324ef33bc6e55f9e15915e98490bd8fcb in / 
# Wed, 11 Jan 2023 02:57:43 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:52:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:52:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 13:52:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 13:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:53:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 13:53:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 13:53:46 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:54:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:54:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 Jan 2023 13:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:55:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15639959ffec1b29b8f88b1e1db3ca0574ca52ee28fd8f3ac6d2cbb1c85fb209`  
		Last Modified: Wed, 11 Jan 2023 03:01:37 GMT  
		Size: 49.2 MB (49233802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426afb0be41a462ca64e39ae6a74ed19ce54db5cd4d8fc00b5094120e8fa8f2`  
		Last Modified: Wed, 11 Jan 2023 14:00:58 GMT  
		Size: 10.9 MB (10902625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71036bab13158db91bd98501b67328211754dad8cac28846bf4aa4ecbde4d658`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e7410b12ea7be4c80024e40f3adcd15efb8dd2b0b24abe4227c4f21cfa894b`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f2c8b362ea16751add95c3717f39e7f30cf2649c3affcc6ae88a08aeab9a5b`  
		Last Modified: Wed, 11 Jan 2023 14:01:21 GMT  
		Size: 184.4 MB (184440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f46ce4b267a4a43fa1378cdd5ec96948d2840335e4ca90ab3100c67516d4c6`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc73cadcad0750f2ced4b8a64f684d077dbc86dfcb490e0705f01e359820dc26`  
		Last Modified: Wed, 11 Jan 2023 14:01:36 GMT  
		Size: 84.4 MB (84392048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2f8d1d96d181162c436accd0a6a33bc249984e8e5ad2fc5476f0e4dd056bcc`  
		Last Modified: Wed, 11 Jan 2023 14:01:28 GMT  
		Size: 335.5 KB (335525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7756844afb4448a1b4c4ef76967534312274fc784844e8f40aa841618908afb6`  
		Last Modified: Wed, 11 Jan 2023 14:01:35 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc647d253f2ca3df07893ab76884b46421df6548be3b133e786b1ca0a309aa`  
		Last Modified: Wed, 11 Jan 2023 14:01:45 GMT  
		Size: 20.8 MB (20819018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:c8cd309e369694d9a472e6669d5860f82ed91e2929da73f809740c323bbb9975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:e7b73f0751dfaf6f249acf7942ba501f8211b94f9e87e67d26a86374d9955f75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359051603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d373974956dd933f9b21ff58168da8fc15cf52a8c6622919719ad011dd850fb4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:36:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22cf93466a9664a9f256c543ada4cb318001c3cf0e631a6e27ed07729dd6355`  
		Last Modified: Tue, 31 Jan 2023 20:09:44 GMT  
		Size: 15.9 MB (15861536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:212560e1cfe592fde12b0668d26a53663f13dedb03e9cbba7662bee9a39fccd9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303343639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba2dedd13d8892bbee3062acd62fb3daafe99715fd9ef3ab3b47ef036e4b47e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f465c6d63ea021516db6106f057d26b8f3ec5b3ea6b8923d4ea13332b4388fd`  
		Last Modified: Wed, 01 Feb 2023 18:55:21 GMT  
		Size: 14.1 MB (14066746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d60eb59c5d99b1d4540311c0096a3f7d82c7b47db6251ade8d926ef82180e0f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338304671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03d47df4b22b25bedb4a11e28c7363ace9cb739f111eb0c7c4b327566dcd67f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:19:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980521b22f06972d2449b80e28733c86c079e2c641b54af5272449178586a1c4`  
		Last Modified: Wed, 01 Feb 2023 19:31:42 GMT  
		Size: 15.5 MB (15457172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:3e95165652987da802b4b70b24a5e68da5381de86a3ee5b5b73a9566c7b0abdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:093dfb05e09d5198362a3f1a69e887c0873c1311bf065fb33816fdc73989743c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343190067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9a9bf50e26daeaaee850bb232ed2a4376df3419ca4ef731987d5afbb0fb13a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:ea8683583e242df0297c9b3921ae5cd4a67ce45139a231f5cd59186407b2af91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289276893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5790bb8151cfbe7c196aa9550d6d53fdfb33e9fb064738db698e49a610ff4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87fe54a6ded5be95e141e9a11f8bd23cc13088e3e01244cf46c98c1e807e72f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d3994a361be4ea5cbd11474d8877364831d3bedc228ad3ac2a76e8d7ce7eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:c32c5e5a412b959c80c3d4a2b6bf0cb8356bacd40b0ee7f9ae450a7aad164e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:564cdfda639887e31fec57bae2734ed4ca6edd85f0054def62cbd6f1964bc6ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.5 MB (463516455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:693bd5ab9e449d41ae5e16846dd16c7226738f20b7635fd51209f2882164f972`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:54 GMT
ADD file:4bf66d4081da52e8b692fcff96aad84d3e68bda4f62e870e8f4803153c70e24c in / 
# Wed, 11 Jan 2023 02:34:55 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:21:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:21:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 17:21:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 17:21:40 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 17:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:22:58 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 17:22:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 17:22:59 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:23:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:23:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 Jan 2023 17:24:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac7f2e1c758675427623d0da4faa88b336c62466c15a98af61efd3f015282f2f`  
		Last Modified: Wed, 11 Jan 2023 02:39:26 GMT  
		Size: 50.4 MB (50448910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed05e22e781556eb3057b10b25e54b8161dad941a5286d7328b50bba2f679b`  
		Last Modified: Wed, 11 Jan 2023 17:29:02 GMT  
		Size: 10.9 MB (10897026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6546cbd4873db6f5862f15a5a02564919836e584e6d1ea33023aa1dd4cdf72f6`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7289081c9d2531b3beccb982cbaefbe997da2cc44528869692cca6bf31ea17`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03333b8952a2f078f37ed6511a22271194ed1d51350d49a57fea72622f4ebac9`  
		Last Modified: Wed, 11 Jan 2023 17:29:33 GMT  
		Size: 239.3 MB (239251419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af920c4677ebb81ba3c51dfea10714e63a1b5819f57dc6c67908a8ad8eccfc`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e754f5425abb4e7c144f985ae140d29c7317db661da308682c81f1a76f3247`  
		Last Modified: Wed, 11 Jan 2023 17:29:51 GMT  
		Size: 86.6 MB (86602948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d11cda2ebbd36d930349879770ec5693b9d903dd36eac0bc8b860aceef9a52`  
		Last Modified: Wed, 11 Jan 2023 17:29:39 GMT  
		Size: 335.5 KB (335525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e3a8dedc38d35e970ad02976d8fd342416f69d45aad155d607eb0f983bd86f`  
		Last Modified: Wed, 11 Jan 2023 17:29:49 GMT  
		Size: 76.0 MB (75978213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0e66a5cf77aca824b7f0db0cd9163dc5c9a7cb258e9a66cfdb16e54c4f82a860
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.4 MB (403397518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec15651108ade29b3d7ce5d9cb4be9a422a29bc16be37bb01990a27cb312d2e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:43 GMT
ADD file:6b2b58305052bb953886c976022efeb324ef33bc6e55f9e15915e98490bd8fcb in / 
# Wed, 11 Jan 2023 02:57:43 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:52:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:52:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 13:52:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 13:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:53:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 13:53:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 13:53:46 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:54:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:54:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 Jan 2023 13:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15639959ffec1b29b8f88b1e1db3ca0574ca52ee28fd8f3ac6d2cbb1c85fb209`  
		Last Modified: Wed, 11 Jan 2023 03:01:37 GMT  
		Size: 49.2 MB (49233802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426afb0be41a462ca64e39ae6a74ed19ce54db5cd4d8fc00b5094120e8fa8f2`  
		Last Modified: Wed, 11 Jan 2023 14:00:58 GMT  
		Size: 10.9 MB (10902625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71036bab13158db91bd98501b67328211754dad8cac28846bf4aa4ecbde4d658`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e7410b12ea7be4c80024e40f3adcd15efb8dd2b0b24abe4227c4f21cfa894b`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f2c8b362ea16751add95c3717f39e7f30cf2649c3affcc6ae88a08aeab9a5b`  
		Last Modified: Wed, 11 Jan 2023 14:01:21 GMT  
		Size: 184.4 MB (184440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f46ce4b267a4a43fa1378cdd5ec96948d2840335e4ca90ab3100c67516d4c6`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc73cadcad0750f2ced4b8a64f684d077dbc86dfcb490e0705f01e359820dc26`  
		Last Modified: Wed, 11 Jan 2023 14:01:36 GMT  
		Size: 84.4 MB (84392048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2f8d1d96d181162c436accd0a6a33bc249984e8e5ad2fc5476f0e4dd056bcc`  
		Last Modified: Wed, 11 Jan 2023 14:01:28 GMT  
		Size: 335.5 KB (335525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7756844afb4448a1b4c4ef76967534312274fc784844e8f40aa841618908afb6`  
		Last Modified: Wed, 11 Jan 2023 14:01:35 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:3e95165652987da802b4b70b24a5e68da5381de86a3ee5b5b73a9566c7b0abdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:093dfb05e09d5198362a3f1a69e887c0873c1311bf065fb33816fdc73989743c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343190067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9a9bf50e26daeaaee850bb232ed2a4376df3419ca4ef731987d5afbb0fb13a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:ea8683583e242df0297c9b3921ae5cd4a67ce45139a231f5cd59186407b2af91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289276893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5790bb8151cfbe7c196aa9550d6d53fdfb33e9fb064738db698e49a610ff4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87fe54a6ded5be95e141e9a11f8bd23cc13088e3e01244cf46c98c1e807e72f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d3994a361be4ea5cbd11474d8877364831d3bedc228ad3ac2a76e8d7ce7eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:bf3a90157f73dd0f76a2b327daa77606d2b83494fa3f1a2a1d124c0623edb1ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:93d0f36b326216ecb88c5059f51ec8177000443ee712c0b7377a9a3d6dbdffa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212300949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb150f893573ded23f1a2f150b8a2783e4e2b65141b7fcfc53704b0642d93f19`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:384f19f5099a3865f3447b895af7e748be7453ab036d8a8ae0ac6d86c371ebcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187935561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a14468079f6c5d9c96ce30eb310845d1c67d556d44cfc2d8bc5d5c2485aa6e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c4e575338068fddfe9bb7e35684d98e1953b4c67e4e4300dc4987e6b13fa300
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205328270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:603c244ecb4f8a0180b03a9dac12a34ad2d284ed0d1acf0f233c15c7887c4b9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:ef9670b73adcd49aa2a0e443d0643c777a536be8b167e2f45358709bf6ba72a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:0627afffdd96ccd98e27b538a11d28be390a0d4d8f2eb6365fd7bd23c0cab9d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300599769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391ea350e41a79a7b58f2a337e94f0841edfd97ffcc436accc4a1a383cc9e2c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:54 GMT
ADD file:4bf66d4081da52e8b692fcff96aad84d3e68bda4f62e870e8f4803153c70e24c in / 
# Wed, 11 Jan 2023 02:34:55 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:21:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:21:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 17:21:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 17:21:40 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 17:21:41 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 17:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:22:58 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 17:22:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 17:22:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac7f2e1c758675427623d0da4faa88b336c62466c15a98af61efd3f015282f2f`  
		Last Modified: Wed, 11 Jan 2023 02:39:26 GMT  
		Size: 50.4 MB (50448910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed05e22e781556eb3057b10b25e54b8161dad941a5286d7328b50bba2f679b`  
		Last Modified: Wed, 11 Jan 2023 17:29:02 GMT  
		Size: 10.9 MB (10897026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6546cbd4873db6f5862f15a5a02564919836e584e6d1ea33023aa1dd4cdf72f6`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7289081c9d2531b3beccb982cbaefbe997da2cc44528869692cca6bf31ea17`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03333b8952a2f078f37ed6511a22271194ed1d51350d49a57fea72622f4ebac9`  
		Last Modified: Wed, 11 Jan 2023 17:29:33 GMT  
		Size: 239.3 MB (239251419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af920c4677ebb81ba3c51dfea10714e63a1b5819f57dc6c67908a8ad8eccfc`  
		Last Modified: Wed, 11 Jan 2023 17:29:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e56bbe844db24cf408a7c6ee90571bc74584a7baa016bbc9ff6a2109d7cf730e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244579296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8907588539207f0ceba27caae7e6008512e905da435233d779efb50f3e483ec5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:43 GMT
ADD file:6b2b58305052bb953886c976022efeb324ef33bc6e55f9e15915e98490bd8fcb in / 
# Wed, 11 Jan 2023 02:57:43 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:52:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:52:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 Jan 2023 13:52:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 Jan 2023 13:52:26 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 Jan 2023 13:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:53:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 11 Jan 2023 13:53:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 Jan 2023 13:53:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:15639959ffec1b29b8f88b1e1db3ca0574ca52ee28fd8f3ac6d2cbb1c85fb209`  
		Last Modified: Wed, 11 Jan 2023 03:01:37 GMT  
		Size: 49.2 MB (49233802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426afb0be41a462ca64e39ae6a74ed19ce54db5cd4d8fc00b5094120e8fa8f2`  
		Last Modified: Wed, 11 Jan 2023 14:00:58 GMT  
		Size: 10.9 MB (10902625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71036bab13158db91bd98501b67328211754dad8cac28846bf4aa4ecbde4d658`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e7410b12ea7be4c80024e40f3adcd15efb8dd2b0b24abe4227c4f21cfa894b`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f2c8b362ea16751add95c3717f39e7f30cf2649c3affcc6ae88a08aeab9a5b`  
		Last Modified: Wed, 11 Jan 2023 14:01:21 GMT  
		Size: 184.4 MB (184440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f46ce4b267a4a43fa1378cdd5ec96948d2840335e4ca90ab3100c67516d4c6`  
		Last Modified: Wed, 11 Jan 2023 14:00:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:bf3a90157f73dd0f76a2b327daa77606d2b83494fa3f1a2a1d124c0623edb1ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:93d0f36b326216ecb88c5059f51ec8177000443ee712c0b7377a9a3d6dbdffa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212300949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb150f893573ded23f1a2f150b8a2783e4e2b65141b7fcfc53704b0642d93f19`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:384f19f5099a3865f3447b895af7e748be7453ab036d8a8ae0ac6d86c371ebcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187935561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a14468079f6c5d9c96ce30eb310845d1c67d556d44cfc2d8bc5d5c2485aa6e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c4e575338068fddfe9bb7e35684d98e1953b4c67e4e4300dc4987e6b13fa300
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205328270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:603c244ecb4f8a0180b03a9dac12a34ad2d284ed0d1acf0f233c15c7887c4b9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:55772449ebbf54e88ac03f9f627f5a6ee395f217c75f137af9eba8e97a233eb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:c9c3d1f71ee0e8129b4b01a60f28940324e0c358c84908882bf74b402402e7cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad19d33c21d926e1d9968c16cc3a41ec7f73c932b979f36182254a7b11e4f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 20:00:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:01:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 20:01:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 20:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b909dcf612dd7292278d51e2aaa53308f2ec52dd9c9bfc178125ce9eceb32`  
		Last Modified: Tue, 31 Jan 2023 20:15:53 GMT  
		Size: 84.9 MB (84915070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a0899e286d8fed703554f8d5887507e2f13408a045817b81dfd9571837879`  
		Last Modified: Tue, 31 Jan 2023 20:15:42 GMT  
		Size: 298.8 KB (298805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07434028456fa3fa86ce7bf3537a45c9126091eb2482bd9db5e474f327edea24`  
		Last Modified: Tue, 31 Jan 2023 20:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8bae09c66c54facf036f53eb067ef4a64073c991441f2a457fffe8b21749b6`  
		Last Modified: Tue, 31 Jan 2023 20:15:45 GMT  
		Size: 22.9 MB (22909564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:32012c4d4d62349c296c0edfac5f930e125f2729726076cc89f4af2a68c9e8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e4649b631a1e68feea5035c3c9858613ae8eb6718d52b879fd9c94d443121c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:54:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:54:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:54:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeba7de9d20a6ea62e137040278c7dc3f6f11ea36ff6d2be71cedec638510414`  
		Last Modified: Tue, 31 Jan 2023 20:05:42 GMT  
		Size: 82.6 MB (82626209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f106db30309da5e784f0b0a54a155708e74aed2a9754505012a584cf0e2f84`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 298.8 KB (298808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ee1ace7724c1f506fa0a46c218d668441abf6f555e4642ad84a6946cf5b23`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f74cada09d2be19f7f229fa3738601396836c483f6629923222ffb8ad06bf`  
		Last Modified: Tue, 31 Jan 2023 20:05:36 GMT  
		Size: 22.3 MB (22322457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:c05ec5e989cafae783794c5ac146e4805ce90df3d3c92af9f6400312ebf6f3e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:d509f66bd5b524c9fc7003156a669c1e2550cb9f991d03d396409d74cff2ace2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092308205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f34c40ea560f00a7db77a42f3340cc1c1f25c5d8f70676bae3a8dace53b0abf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 20:00:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:01:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 20:01:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 20:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:05:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b909dcf612dd7292278d51e2aaa53308f2ec52dd9c9bfc178125ce9eceb32`  
		Last Modified: Tue, 31 Jan 2023 20:15:53 GMT  
		Size: 84.9 MB (84915070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a0899e286d8fed703554f8d5887507e2f13408a045817b81dfd9571837879`  
		Last Modified: Tue, 31 Jan 2023 20:15:42 GMT  
		Size: 298.8 KB (298805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07434028456fa3fa86ce7bf3537a45c9126091eb2482bd9db5e474f327edea24`  
		Last Modified: Tue, 31 Jan 2023 20:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8bae09c66c54facf036f53eb067ef4a64073c991441f2a457fffe8b21749b6`  
		Last Modified: Tue, 31 Jan 2023 20:15:45 GMT  
		Size: 22.9 MB (22909564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b8b9412f2303f6bb09baa054a15883e6586bfea64b4f4723f070d7b68ae2b5`  
		Last Modified: Tue, 31 Jan 2023 20:17:42 GMT  
		Size: 829.3 MB (829259969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:12371d40203f46efb145311c349811056566982015f64f81f4bfa181ae00fc22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043678477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68d94c1e9f0f17dec968f5bc833f3cfd2f5baae3f93d0dbc7a7767a0a3c58b8b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:54:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:54:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:54:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:56:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeba7de9d20a6ea62e137040278c7dc3f6f11ea36ff6d2be71cedec638510414`  
		Last Modified: Tue, 31 Jan 2023 20:05:42 GMT  
		Size: 82.6 MB (82626209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f106db30309da5e784f0b0a54a155708e74aed2a9754505012a584cf0e2f84`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 298.8 KB (298808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ee1ace7724c1f506fa0a46c218d668441abf6f555e4642ad84a6946cf5b23`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f74cada09d2be19f7f229fa3738601396836c483f6629923222ffb8ad06bf`  
		Last Modified: Tue, 31 Jan 2023 20:05:36 GMT  
		Size: 22.3 MB (22322457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc81d6699a8d641c413a1ea474ef4bcc825469e939fdaf9aa78dc3931ac043f`  
		Last Modified: Tue, 31 Jan 2023 20:07:09 GMT  
		Size: 788.0 MB (787993367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:c05ec5e989cafae783794c5ac146e4805ce90df3d3c92af9f6400312ebf6f3e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:d509f66bd5b524c9fc7003156a669c1e2550cb9f991d03d396409d74cff2ace2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092308205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f34c40ea560f00a7db77a42f3340cc1c1f25c5d8f70676bae3a8dace53b0abf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 20:00:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:01:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 20:01:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 20:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:05:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b909dcf612dd7292278d51e2aaa53308f2ec52dd9c9bfc178125ce9eceb32`  
		Last Modified: Tue, 31 Jan 2023 20:15:53 GMT  
		Size: 84.9 MB (84915070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a0899e286d8fed703554f8d5887507e2f13408a045817b81dfd9571837879`  
		Last Modified: Tue, 31 Jan 2023 20:15:42 GMT  
		Size: 298.8 KB (298805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07434028456fa3fa86ce7bf3537a45c9126091eb2482bd9db5e474f327edea24`  
		Last Modified: Tue, 31 Jan 2023 20:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8bae09c66c54facf036f53eb067ef4a64073c991441f2a457fffe8b21749b6`  
		Last Modified: Tue, 31 Jan 2023 20:15:45 GMT  
		Size: 22.9 MB (22909564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b8b9412f2303f6bb09baa054a15883e6586bfea64b4f4723f070d7b68ae2b5`  
		Last Modified: Tue, 31 Jan 2023 20:17:42 GMT  
		Size: 829.3 MB (829259969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:12371d40203f46efb145311c349811056566982015f64f81f4bfa181ae00fc22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043678477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68d94c1e9f0f17dec968f5bc833f3cfd2f5baae3f93d0dbc7a7767a0a3c58b8b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:54:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:54:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:54:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:56:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeba7de9d20a6ea62e137040278c7dc3f6f11ea36ff6d2be71cedec638510414`  
		Last Modified: Tue, 31 Jan 2023 20:05:42 GMT  
		Size: 82.6 MB (82626209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f106db30309da5e784f0b0a54a155708e74aed2a9754505012a584cf0e2f84`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 298.8 KB (298808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ee1ace7724c1f506fa0a46c218d668441abf6f555e4642ad84a6946cf5b23`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f74cada09d2be19f7f229fa3738601396836c483f6629923222ffb8ad06bf`  
		Last Modified: Tue, 31 Jan 2023 20:05:36 GMT  
		Size: 22.3 MB (22322457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc81d6699a8d641c413a1ea474ef4bcc825469e939fdaf9aa78dc3931ac043f`  
		Last Modified: Tue, 31 Jan 2023 20:07:09 GMT  
		Size: 788.0 MB (787993367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:55772449ebbf54e88ac03f9f627f5a6ee395f217c75f137af9eba8e97a233eb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c9c3d1f71ee0e8129b4b01a60f28940324e0c358c84908882bf74b402402e7cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad19d33c21d926e1d9968c16cc3a41ec7f73c932b979f36182254a7b11e4f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 20:00:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:01:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 20:01:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 20:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b909dcf612dd7292278d51e2aaa53308f2ec52dd9c9bfc178125ce9eceb32`  
		Last Modified: Tue, 31 Jan 2023 20:15:53 GMT  
		Size: 84.9 MB (84915070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a0899e286d8fed703554f8d5887507e2f13408a045817b81dfd9571837879`  
		Last Modified: Tue, 31 Jan 2023 20:15:42 GMT  
		Size: 298.8 KB (298805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07434028456fa3fa86ce7bf3537a45c9126091eb2482bd9db5e474f327edea24`  
		Last Modified: Tue, 31 Jan 2023 20:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8bae09c66c54facf036f53eb067ef4a64073c991441f2a457fffe8b21749b6`  
		Last Modified: Tue, 31 Jan 2023 20:15:45 GMT  
		Size: 22.9 MB (22909564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:32012c4d4d62349c296c0edfac5f930e125f2729726076cc89f4af2a68c9e8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e4649b631a1e68feea5035c3c9858613ae8eb6718d52b879fd9c94d443121c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:54:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:54:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:54:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeba7de9d20a6ea62e137040278c7dc3f6f11ea36ff6d2be71cedec638510414`  
		Last Modified: Tue, 31 Jan 2023 20:05:42 GMT  
		Size: 82.6 MB (82626209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f106db30309da5e784f0b0a54a155708e74aed2a9754505012a584cf0e2f84`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 298.8 KB (298808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ee1ace7724c1f506fa0a46c218d668441abf6f555e4642ad84a6946cf5b23`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f74cada09d2be19f7f229fa3738601396836c483f6629923222ffb8ad06bf`  
		Last Modified: Tue, 31 Jan 2023 20:05:36 GMT  
		Size: 22.3 MB (22322457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:55772449ebbf54e88ac03f9f627f5a6ee395f217c75f137af9eba8e97a233eb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c9c3d1f71ee0e8129b4b01a60f28940324e0c358c84908882bf74b402402e7cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad19d33c21d926e1d9968c16cc3a41ec7f73c932b979f36182254a7b11e4f22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 20:00:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:01:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 20:01:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 20:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b909dcf612dd7292278d51e2aaa53308f2ec52dd9c9bfc178125ce9eceb32`  
		Last Modified: Tue, 31 Jan 2023 20:15:53 GMT  
		Size: 84.9 MB (84915070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a0899e286d8fed703554f8d5887507e2f13408a045817b81dfd9571837879`  
		Last Modified: Tue, 31 Jan 2023 20:15:42 GMT  
		Size: 298.8 KB (298805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07434028456fa3fa86ce7bf3537a45c9126091eb2482bd9db5e474f327edea24`  
		Last Modified: Tue, 31 Jan 2023 20:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8bae09c66c54facf036f53eb067ef4a64073c991441f2a457fffe8b21749b6`  
		Last Modified: Tue, 31 Jan 2023 20:15:45 GMT  
		Size: 22.9 MB (22909564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:32012c4d4d62349c296c0edfac5f930e125f2729726076cc89f4af2a68c9e8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e4649b631a1e68feea5035c3c9858613ae8eb6718d52b879fd9c94d443121c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:54:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:54:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:54:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeba7de9d20a6ea62e137040278c7dc3f6f11ea36ff6d2be71cedec638510414`  
		Last Modified: Tue, 31 Jan 2023 20:05:42 GMT  
		Size: 82.6 MB (82626209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f106db30309da5e784f0b0a54a155708e74aed2a9754505012a584cf0e2f84`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 298.8 KB (298808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ee1ace7724c1f506fa0a46c218d668441abf6f555e4642ad84a6946cf5b23`  
		Last Modified: Tue, 31 Jan 2023 20:05:33 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f74cada09d2be19f7f229fa3738601396836c483f6629923222ffb8ad06bf`  
		Last Modified: Tue, 31 Jan 2023 20:05:36 GMT  
		Size: 22.3 MB (22322457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:bb9356997c6244f4e42b8db21ec67a340560654f047e34529f14d8079be66b75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:88d8e636517283d5770a6934daa23f3085df98f2a7399f947111b5f48ef741f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154922349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07897d4d91378e7373d7bffa34dab18c8033a18f0d9288f05eaf42654eef357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad9dbd6cff619bb80c3036c9d42bbc7adac7b0e272cc8c59bd8b3a978762f3bc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150435232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc1265677e89579bd11423bd7f77b2627c340c97ed901514d630bcafc22a746a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:bb9356997c6244f4e42b8db21ec67a340560654f047e34529f14d8079be66b75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:88d8e636517283d5770a6934daa23f3085df98f2a7399f947111b5f48ef741f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154922349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07897d4d91378e7373d7bffa34dab18c8033a18f0d9288f05eaf42654eef357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad9dbd6cff619bb80c3036c9d42bbc7adac7b0e272cc8c59bd8b3a978762f3bc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150435232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc1265677e89579bd11423bd7f77b2627c340c97ed901514d630bcafc22a746a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:38:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:38:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:38:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:53:11 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 19:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:53:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:53:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:53:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4a5b8d8fdbef5d71aa0cf199586790c9535d7fa75b076e05a33f472ccde52`  
		Last Modified: Tue, 31 Jan 2023 20:02:48 GMT  
		Size: 1.2 MB (1171081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1bef2f7844fee60225a5be2ce107f756ec6251ec81ac2cd4038469d8535a06`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 3.8 MB (3801649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292acdedefe1520d32569a3a55871b34f5ca8a34fe7ebb4c18cbe9e276949a5c`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f2ad17610e16ad4b4439447719d0aaf2954f99cec558e4676499371401a2f`  
		Last Modified: Tue, 31 Jan 2023 20:02:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b405443e82c265918d1c4dca7e006b87e9fb4ae0abefccc8ce4f1e26cad7a`  
		Last Modified: Tue, 31 Jan 2023 20:05:25 GMT  
		Size: 117.1 MB (117075112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470885452e3340b2399ae79e9dc643b3eb21f12533f06183145e0be5a2c5ca02`  
		Last Modified: Tue, 31 Jan 2023 20:05:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
