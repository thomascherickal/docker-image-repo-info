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
$ docker pull ros@sha256:4ba8f08ed1acf4b3384435a777ad4b5d5b8c37a027001460b697d5318b0c3076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:2d7bdfc0fabdb42c3b0ccae337b6448f5ea263e5d863ad6ff4138d54ef80f418
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250912800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8337d52bce89c16354cd2d09f84d78612ebe9f63d68e64827f0a9f4fc9e9fe54`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:10:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:10:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed015d15add357da85905f59d7481744b4f675188a10028320ae711bf62333`  
		Last Modified: Fri, 09 Dec 2022 05:37:34 GMT  
		Size: 73.3 MB (73329408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cee15e997c7e8f91044ddbe298b6ae390c6962b7f91c7285e0a1977ecaa878`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa7c53a8838d51439e8aeeefc7232ae9a6f4fff49431a10043cf435d7e372`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 2.4 KB (2424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379ba7f826eed63a7ec51c723d73f5dcc9fadb1dcd3d16a2454ea55eba5563c`  
		Last Modified: Fri, 09 Dec 2022 05:37:27 GMT  
		Size: 21.7 MB (21661894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3bd2807282747665977c9307e11b8ec7711e1c2e8c27d198e95bfeca082c50c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226768906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7587310c6b44ff3da224dbd8e03b7d33afb0543ab73625ea09bbceb64ee86380`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:58:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:58:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 02:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5f1a3dce8a3f2f12beb55a97c38fd532de4ada449ba5b750db310a4aa1bed8`  
		Last Modified: Fri, 09 Dec 2022 03:25:50 GMT  
		Size: 67.7 MB (67675837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723621fb31f36278e19e21bda4d6500be7e52051ac4770104af43a73b63378e`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839a08922d0c890f3b65207c8b706707fb2fa295f2e885d0ce6ac9a8eed4af7`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997775b4aaae4594dd1bc521b063cd4bbdb0403cc5a2946344515519f7dff081`  
		Last Modified: Fri, 09 Dec 2022 03:25:44 GMT  
		Size: 20.4 MB (20374509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:4ba8f08ed1acf4b3384435a777ad4b5d5b8c37a027001460b697d5318b0c3076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2d7bdfc0fabdb42c3b0ccae337b6448f5ea263e5d863ad6ff4138d54ef80f418
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250912800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8337d52bce89c16354cd2d09f84d78612ebe9f63d68e64827f0a9f4fc9e9fe54`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:10:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:10:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed015d15add357da85905f59d7481744b4f675188a10028320ae711bf62333`  
		Last Modified: Fri, 09 Dec 2022 05:37:34 GMT  
		Size: 73.3 MB (73329408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cee15e997c7e8f91044ddbe298b6ae390c6962b7f91c7285e0a1977ecaa878`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa7c53a8838d51439e8aeeefc7232ae9a6f4fff49431a10043cf435d7e372`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 2.4 KB (2424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379ba7f826eed63a7ec51c723d73f5dcc9fadb1dcd3d16a2454ea55eba5563c`  
		Last Modified: Fri, 09 Dec 2022 05:37:27 GMT  
		Size: 21.7 MB (21661894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3bd2807282747665977c9307e11b8ec7711e1c2e8c27d198e95bfeca082c50c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226768906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7587310c6b44ff3da224dbd8e03b7d33afb0543ab73625ea09bbceb64ee86380`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:58:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:58:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 02:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5f1a3dce8a3f2f12beb55a97c38fd532de4ada449ba5b750db310a4aa1bed8`  
		Last Modified: Fri, 09 Dec 2022 03:25:50 GMT  
		Size: 67.7 MB (67675837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723621fb31f36278e19e21bda4d6500be7e52051ac4770104af43a73b63378e`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839a08922d0c890f3b65207c8b706707fb2fa295f2e885d0ce6ac9a8eed4af7`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997775b4aaae4594dd1bc521b063cd4bbdb0403cc5a2946344515519f7dff081`  
		Last Modified: Fri, 09 Dec 2022 03:25:44 GMT  
		Size: 20.4 MB (20374509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:4ba8f08ed1acf4b3384435a777ad4b5d5b8c37a027001460b697d5318b0c3076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:2d7bdfc0fabdb42c3b0ccae337b6448f5ea263e5d863ad6ff4138d54ef80f418
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250912800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8337d52bce89c16354cd2d09f84d78612ebe9f63d68e64827f0a9f4fc9e9fe54`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:10:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:10:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed015d15add357da85905f59d7481744b4f675188a10028320ae711bf62333`  
		Last Modified: Fri, 09 Dec 2022 05:37:34 GMT  
		Size: 73.3 MB (73329408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cee15e997c7e8f91044ddbe298b6ae390c6962b7f91c7285e0a1977ecaa878`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa7c53a8838d51439e8aeeefc7232ae9a6f4fff49431a10043cf435d7e372`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 2.4 KB (2424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379ba7f826eed63a7ec51c723d73f5dcc9fadb1dcd3d16a2454ea55eba5563c`  
		Last Modified: Fri, 09 Dec 2022 05:37:27 GMT  
		Size: 21.7 MB (21661894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3bd2807282747665977c9307e11b8ec7711e1c2e8c27d198e95bfeca082c50c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226768906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7587310c6b44ff3da224dbd8e03b7d33afb0543ab73625ea09bbceb64ee86380`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:58:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:58:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 02:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5f1a3dce8a3f2f12beb55a97c38fd532de4ada449ba5b750db310a4aa1bed8`  
		Last Modified: Fri, 09 Dec 2022 03:25:50 GMT  
		Size: 67.7 MB (67675837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723621fb31f36278e19e21bda4d6500be7e52051ac4770104af43a73b63378e`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839a08922d0c890f3b65207c8b706707fb2fa295f2e885d0ce6ac9a8eed4af7`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997775b4aaae4594dd1bc521b063cd4bbdb0403cc5a2946344515519f7dff081`  
		Last Modified: Fri, 09 Dec 2022 03:25:44 GMT  
		Size: 20.4 MB (20374509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:f3f6c436ed7a1d454f1e85e9e37c099abee2917e739cd01e5a850675bd1fff4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:059bdcd9c674d82d5a5a037a55d565c6e6252e3e00bef30005b753d9538c4df7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155643105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c42f239d3e226d0baa55cd450366509efbfcef2e7368bbc9b12799dfb855654`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:29b97362e854a99899eec52f0de8396791017055b7abe8337ccb71f41b56978f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138440171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d9cdb197b2bedf84ca2c9b357ce0f9c3866e65896f79887746579223e5eecd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:f3f6c436ed7a1d454f1e85e9e37c099abee2917e739cd01e5a850675bd1fff4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:059bdcd9c674d82d5a5a037a55d565c6e6252e3e00bef30005b753d9538c4df7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155643105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c42f239d3e226d0baa55cd450366509efbfcef2e7368bbc9b12799dfb855654`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:29b97362e854a99899eec52f0de8396791017055b7abe8337ccb71f41b56978f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138440171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d9cdb197b2bedf84ca2c9b357ce0f9c3866e65896f79887746579223e5eecd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:cbd3e5f82e4579b530ed3520606c5948cb59424563db8cbad2f84403ef2f9bd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:13dacc3393e00d5d4c450f5fc6a2f2a66e7b306fb7c72227cbc37a22ad142ec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349023089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fc011ac8df8d790efa40b61f2b8ca756f822bd6ffd7044d9c91b2bb284d531`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:10:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:10:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:11:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 05:11:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:11:28 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 05:11:28 GMT
ENV ROS2_DISTRO=foxy
# Fri, 09 Dec 2022 05:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:12:05 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed015d15add357da85905f59d7481744b4f675188a10028320ae711bf62333`  
		Last Modified: Fri, 09 Dec 2022 05:37:34 GMT  
		Size: 73.3 MB (73329408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cee15e997c7e8f91044ddbe298b6ae390c6962b7f91c7285e0a1977ecaa878`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa7c53a8838d51439e8aeeefc7232ae9a6f4fff49431a10043cf435d7e372`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 2.4 KB (2424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379ba7f826eed63a7ec51c723d73f5dcc9fadb1dcd3d16a2454ea55eba5563c`  
		Last Modified: Fri, 09 Dec 2022 05:37:27 GMT  
		Size: 21.7 MB (21661894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daea7a721eeb379e4e148b82ac9e7b7e3f66a087710e6bc04c4c213267404671`  
		Last Modified: Fri, 09 Dec 2022 05:37:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ee9c3b3f8f01fec0572530d8f497623409042c0eb8c8c0b0bb3879cafb84e5`  
		Last Modified: Fri, 09 Dec 2022 05:37:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13c2b5c413a8e4e24d9972cc239f10d5d43ee296d220d117d961a1f05ce5dc4`  
		Last Modified: Fri, 09 Dec 2022 05:38:00 GMT  
		Size: 76.4 MB (76435948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dbfb1da6fa97bd4c5263d1c48dc8b96615a0a8cbc69faac5c1f045e14b17d`  
		Last Modified: Fri, 09 Dec 2022 05:37:50 GMT  
		Size: 21.7 MB (21673714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e830f96a7f61c062254545c50d276c369eb21f6683b3bd3873d70b1247466`  
		Last Modified: Fri, 09 Dec 2022 05:37:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:010226ef11433c6a73fc40fd0970babc2f6586adac27f5e7786a5e1df311d068
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317593291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067a40eb07c458c9510406345e281cb33097f60e7c08061b71d51e5c57f20344`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:58:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:58:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 02:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:59:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:59:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:59:01 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 02:59:01 GMT
ENV ROS2_DISTRO=foxy
# Fri, 09 Dec 2022 02:59:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:59:31 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5f1a3dce8a3f2f12beb55a97c38fd532de4ada449ba5b750db310a4aa1bed8`  
		Last Modified: Fri, 09 Dec 2022 03:25:50 GMT  
		Size: 67.7 MB (67675837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723621fb31f36278e19e21bda4d6500be7e52051ac4770104af43a73b63378e`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839a08922d0c890f3b65207c8b706707fb2fa295f2e885d0ce6ac9a8eed4af7`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997775b4aaae4594dd1bc521b063cd4bbdb0403cc5a2946344515519f7dff081`  
		Last Modified: Fri, 09 Dec 2022 03:25:44 GMT  
		Size: 20.4 MB (20374509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7aa536f1a3b87a1484b34e013e3607aaaefded6a8b4630f27d36a87f473149`  
		Last Modified: Fri, 09 Dec 2022 03:26:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43235d137847611a76f6b6f03f1d99a5b19fd153b482ac53fc009fde95bdd6c2`  
		Last Modified: Fri, 09 Dec 2022 03:26:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b949780ead758ed08f810c4fc2dd16232be0ee168a0f63172105a739dc6bd28f`  
		Last Modified: Fri, 09 Dec 2022 03:26:15 GMT  
		Size: 76.5 MB (76498961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5bb53fdc720e28ffa9ff5fdfe37b66f6802eab8d7bb04b3070fe51b33b0764`  
		Last Modified: Fri, 09 Dec 2022 03:26:04 GMT  
		Size: 14.3 MB (14324793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c8d0e73fcbef93589d60ce11fb61b011595f8709c145e30b1957d94c6a099b`  
		Last Modified: Fri, 09 Dec 2022 03:26:01 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:cbd3e5f82e4579b530ed3520606c5948cb59424563db8cbad2f84403ef2f9bd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:13dacc3393e00d5d4c450f5fc6a2f2a66e7b306fb7c72227cbc37a22ad142ec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349023089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fc011ac8df8d790efa40b61f2b8ca756f822bd6ffd7044d9c91b2bb284d531`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 05:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:20 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:10:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:10:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:10:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:10:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:10:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:11:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 05:11:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:11:28 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 05:11:28 GMT
ENV ROS2_DISTRO=foxy
# Fri, 09 Dec 2022 05:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:12:05 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa0fd25479e87bf4b59c713667040fe65a73ecb8fe6c15a500608bd704c85e`  
		Last Modified: Fri, 09 Dec 2022 05:37:15 GMT  
		Size: 120.4 MB (120357554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22220a302ca51863184e466e3f144a75bd9e92b97eeeec34ee8cb4557a0255e0`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed015d15add357da85905f59d7481744b4f675188a10028320ae711bf62333`  
		Last Modified: Fri, 09 Dec 2022 05:37:34 GMT  
		Size: 73.3 MB (73329408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cee15e997c7e8f91044ddbe298b6ae390c6962b7f91c7285e0a1977ecaa878`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa7c53a8838d51439e8aeeefc7232ae9a6f4fff49431a10043cf435d7e372`  
		Last Modified: Fri, 09 Dec 2022 05:37:24 GMT  
		Size: 2.4 KB (2424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379ba7f826eed63a7ec51c723d73f5dcc9fadb1dcd3d16a2454ea55eba5563c`  
		Last Modified: Fri, 09 Dec 2022 05:37:27 GMT  
		Size: 21.7 MB (21661894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daea7a721eeb379e4e148b82ac9e7b7e3f66a087710e6bc04c4c213267404671`  
		Last Modified: Fri, 09 Dec 2022 05:37:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ee9c3b3f8f01fec0572530d8f497623409042c0eb8c8c0b0bb3879cafb84e5`  
		Last Modified: Fri, 09 Dec 2022 05:37:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13c2b5c413a8e4e24d9972cc239f10d5d43ee296d220d117d961a1f05ce5dc4`  
		Last Modified: Fri, 09 Dec 2022 05:38:00 GMT  
		Size: 76.4 MB (76435948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dbfb1da6fa97bd4c5263d1c48dc8b96615a0a8cbc69faac5c1f045e14b17d`  
		Last Modified: Fri, 09 Dec 2022 05:37:50 GMT  
		Size: 21.7 MB (21673714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e830f96a7f61c062254545c50d276c369eb21f6683b3bd3873d70b1247466`  
		Last Modified: Fri, 09 Dec 2022 05:37:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:010226ef11433c6a73fc40fd0970babc2f6586adac27f5e7786a5e1df311d068
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317593291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067a40eb07c458c9510406345e281cb33097f60e7c08061b71d51e5c57f20344`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 09 Dec 2022 02:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 02:58:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:58:08 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:58:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:58:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 02:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:59:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:59:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:59:01 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 02:59:01 GMT
ENV ROS2_DISTRO=foxy
# Fri, 09 Dec 2022 02:59:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:59:31 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b03de35f99ecdd5e2c6b9edc57c370fc1235d49e5e8f0924ed85b7135606a4`  
		Last Modified: Fri, 09 Dec 2022 03:25:33 GMT  
		Size: 104.6 MB (104558778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2e2e21c49243bd9f7d395063bbef5d9e86be8f2fb787901b8ca504bae3123a`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5f1a3dce8a3f2f12beb55a97c38fd532de4ada449ba5b750db310a4aa1bed8`  
		Last Modified: Fri, 09 Dec 2022 03:25:50 GMT  
		Size: 67.7 MB (67675837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723621fb31f36278e19e21bda4d6500be7e52051ac4770104af43a73b63378e`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 276.0 KB (275969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839a08922d0c890f3b65207c8b706707fb2fa295f2e885d0ce6ac9a8eed4af7`  
		Last Modified: Fri, 09 Dec 2022 03:25:41 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997775b4aaae4594dd1bc521b063cd4bbdb0403cc5a2946344515519f7dff081`  
		Last Modified: Fri, 09 Dec 2022 03:25:44 GMT  
		Size: 20.4 MB (20374509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7aa536f1a3b87a1484b34e013e3607aaaefded6a8b4630f27d36a87f473149`  
		Last Modified: Fri, 09 Dec 2022 03:26:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43235d137847611a76f6b6f03f1d99a5b19fd153b482ac53fc009fde95bdd6c2`  
		Last Modified: Fri, 09 Dec 2022 03:26:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b949780ead758ed08f810c4fc2dd16232be0ee168a0f63172105a739dc6bd28f`  
		Last Modified: Fri, 09 Dec 2022 03:26:15 GMT  
		Size: 76.5 MB (76498961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5bb53fdc720e28ffa9ff5fdfe37b66f6802eab8d7bb04b3070fe51b33b0764`  
		Last Modified: Fri, 09 Dec 2022 03:26:04 GMT  
		Size: 14.3 MB (14324793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c8d0e73fcbef93589d60ce11fb61b011595f8709c145e30b1957d94c6a099b`  
		Last Modified: Fri, 09 Dec 2022 03:26:01 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:3347ff1ddfb2b8aca5cd2ebc6a108acaae8393b47806c01d9af4509945d39c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:213a8265f0b42cabd610b3dcf989e651415468dad57312b75052caf2927b8333
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234898602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249ed8c3049c352e3d5531f9dab5b02e0fcba05125a7ef1daf7558b76d35a309`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:13:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cb9e3c282d37d8c15c88800d126b8e236c391f7580ae4075c9eb1af48cd2be`  
		Last Modified: Fri, 09 Dec 2022 05:38:45 GMT  
		Size: 73.3 MB (73282784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def0d48a89f17574beb102c43e3542f8835cfcf9f91ceca92952f442cf8494b8`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 286.4 KB (286430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4223ffc392fc5e9b4afd8b6613332f44d08db8721ace9f392d0ab22e7a1b1a0`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985a64d72dd41c16338473f48d90cbc5a2c63414c9e533bf85d8644dc78a57f`  
		Last Modified: Fri, 09 Dec 2022 05:38:38 GMT  
		Size: 22.1 MB (22138677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:43fbc7b16ce996cf725cc9c5f920d42922afb6a9c42d7d600129c9854913d248
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223584988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b137f52b5959321903f0cf7396cbf64b961560f6b0ad41b062a1cd805f8c4fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:00:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:00:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6350e2bac55c944dd34bc29e73fbc018fec2cf5e94689af115f8f54b5fec657b`  
		Last Modified: Fri, 09 Dec 2022 03:26:59 GMT  
		Size: 67.6 MB (67619151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a7b4cc4ed2f5afbc7072d331d05a7d4434dfabbef418886de0d8eb7de662f1`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 286.4 KB (286436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3991e0369f7386b610317863996480f39b063fff1a1b32babcb037cf7643a7`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345475a6e74d5f984d572de5f7122f7bad7e4b7a22e9914852dc4297ce04929f`  
		Last Modified: Fri, 09 Dec 2022 03:26:54 GMT  
		Size: 21.5 MB (21474900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:3347ff1ddfb2b8aca5cd2ebc6a108acaae8393b47806c01d9af4509945d39c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:213a8265f0b42cabd610b3dcf989e651415468dad57312b75052caf2927b8333
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234898602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249ed8c3049c352e3d5531f9dab5b02e0fcba05125a7ef1daf7558b76d35a309`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:13:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cb9e3c282d37d8c15c88800d126b8e236c391f7580ae4075c9eb1af48cd2be`  
		Last Modified: Fri, 09 Dec 2022 05:38:45 GMT  
		Size: 73.3 MB (73282784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def0d48a89f17574beb102c43e3542f8835cfcf9f91ceca92952f442cf8494b8`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 286.4 KB (286430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4223ffc392fc5e9b4afd8b6613332f44d08db8721ace9f392d0ab22e7a1b1a0`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985a64d72dd41c16338473f48d90cbc5a2c63414c9e533bf85d8644dc78a57f`  
		Last Modified: Fri, 09 Dec 2022 05:38:38 GMT  
		Size: 22.1 MB (22138677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:43fbc7b16ce996cf725cc9c5f920d42922afb6a9c42d7d600129c9854913d248
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223584988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b137f52b5959321903f0cf7396cbf64b961560f6b0ad41b062a1cd805f8c4fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:00:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:00:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6350e2bac55c944dd34bc29e73fbc018fec2cf5e94689af115f8f54b5fec657b`  
		Last Modified: Fri, 09 Dec 2022 03:26:59 GMT  
		Size: 67.6 MB (67619151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a7b4cc4ed2f5afbc7072d331d05a7d4434dfabbef418886de0d8eb7de662f1`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 286.4 KB (286436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3991e0369f7386b610317863996480f39b063fff1a1b32babcb037cf7643a7`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345475a6e74d5f984d572de5f7122f7bad7e4b7a22e9914852dc4297ce04929f`  
		Last Modified: Fri, 09 Dec 2022 03:26:54 GMT  
		Size: 21.5 MB (21474900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:3347ff1ddfb2b8aca5cd2ebc6a108acaae8393b47806c01d9af4509945d39c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:213a8265f0b42cabd610b3dcf989e651415468dad57312b75052caf2927b8333
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234898602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249ed8c3049c352e3d5531f9dab5b02e0fcba05125a7ef1daf7558b76d35a309`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:13:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cb9e3c282d37d8c15c88800d126b8e236c391f7580ae4075c9eb1af48cd2be`  
		Last Modified: Fri, 09 Dec 2022 05:38:45 GMT  
		Size: 73.3 MB (73282784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def0d48a89f17574beb102c43e3542f8835cfcf9f91ceca92952f442cf8494b8`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 286.4 KB (286430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4223ffc392fc5e9b4afd8b6613332f44d08db8721ace9f392d0ab22e7a1b1a0`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985a64d72dd41c16338473f48d90cbc5a2c63414c9e533bf85d8644dc78a57f`  
		Last Modified: Fri, 09 Dec 2022 05:38:38 GMT  
		Size: 22.1 MB (22138677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:43fbc7b16ce996cf725cc9c5f920d42922afb6a9c42d7d600129c9854913d248
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223584988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b137f52b5959321903f0cf7396cbf64b961560f6b0ad41b062a1cd805f8c4fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:00:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:00:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6350e2bac55c944dd34bc29e73fbc018fec2cf5e94689af115f8f54b5fec657b`  
		Last Modified: Fri, 09 Dec 2022 03:26:59 GMT  
		Size: 67.6 MB (67619151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a7b4cc4ed2f5afbc7072d331d05a7d4434dfabbef418886de0d8eb7de662f1`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 286.4 KB (286436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3991e0369f7386b610317863996480f39b063fff1a1b32babcb037cf7643a7`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345475a6e74d5f984d572de5f7122f7bad7e4b7a22e9914852dc4297ce04929f`  
		Last Modified: Fri, 09 Dec 2022 03:26:54 GMT  
		Size: 21.5 MB (21474900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:69d9c967022653f8bd8b092fe2953e3af61c3d93b03e0f579b2e0df58b297ed7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:14b856e24a18927834f428e346de493c371b18eb25dd0280138d8d1e263925b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139188301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db77abc4432149210c5f25b1753f567f5a54b113d439df6b6e25930bd38f780`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a86e32bb5af6ff2bacb44381af2172b3d2ffe843fdacd5e1367e89f0dd94154
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134202092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18d0a36965cfcbdc1b23e9bc747b950f719ec6126770e1b2e8fa2e724364f0a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:69d9c967022653f8bd8b092fe2953e3af61c3d93b03e0f579b2e0df58b297ed7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:14b856e24a18927834f428e346de493c371b18eb25dd0280138d8d1e263925b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139188301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db77abc4432149210c5f25b1753f567f5a54b113d439df6b6e25930bd38f780`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a86e32bb5af6ff2bacb44381af2172b3d2ffe843fdacd5e1367e89f0dd94154
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134202092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18d0a36965cfcbdc1b23e9bc747b950f719ec6126770e1b2e8fa2e724364f0a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:54f193b88f9efbd93a8281d7631c8ca87a1c3bc0c7274b6b63ed5805f5bccac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:951b800e7f0881c6436ef345689ac2f1da9750afaaca8f00fbd773b02fef3275
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330100546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e657f26897db359d6ce72d70068770a0a3eebb04a19d7bca0ad845929a9dd61`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:13:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 05:13:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:13:53 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 05:13:53 GMT
ENV ROS2_DISTRO=galactic
# Fri, 09 Dec 2022 05:14:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 21:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.4-1*     ros-galactic-demo-nodes-py=0.14.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 21:12:34 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cb9e3c282d37d8c15c88800d126b8e236c391f7580ae4075c9eb1af48cd2be`  
		Last Modified: Fri, 09 Dec 2022 05:38:45 GMT  
		Size: 73.3 MB (73282784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def0d48a89f17574beb102c43e3542f8835cfcf9f91ceca92952f442cf8494b8`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 286.4 KB (286430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4223ffc392fc5e9b4afd8b6613332f44d08db8721ace9f392d0ab22e7a1b1a0`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985a64d72dd41c16338473f48d90cbc5a2c63414c9e533bf85d8644dc78a57f`  
		Last Modified: Fri, 09 Dec 2022 05:38:38 GMT  
		Size: 22.1 MB (22138677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a516984ebca41375d3fdc82de7f43b9d8565c16de9d1e92073a45ec5e4de152`  
		Last Modified: Fri, 09 Dec 2022 05:38:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8344261bd56aeff273ec59554955f180c54c8a91313cac7b19b85ac1da1e9849`  
		Last Modified: Fri, 09 Dec 2022 05:38:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3d8a6822222d0f78e01589432f4fd8704e8419dae46b19c8b7121212bd369b`  
		Last Modified: Fri, 09 Dec 2022 05:39:10 GMT  
		Size: 78.7 MB (78709342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbf627443c5d8d8f5d4da4951347df2b77406e2292b0269de43b33fedc0471`  
		Last Modified: Mon, 12 Dec 2022 21:13:58 GMT  
		Size: 16.5 MB (16491975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca66a22ff38141d8f6ae0c4bf96c37d5424b1520b7b4b7a309e98e7a3669826`  
		Last Modified: Mon, 12 Dec 2022 21:13:55 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:01866ba9e9b22b8afe18221e789b3d0f4b90bf42400d29b928ede1afe6d3e417
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318266148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7646a811d85b21b2ba5e1c69cc35e79bc54d4a3b6ebb15bccefd852a34dbab97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:00:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:00:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 03:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:00:55 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 03:00:55 GMT
ENV ROS2_DISTRO=galactic
# Fri, 09 Dec 2022 03:01:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 20:11:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.4-1*     ros-galactic-demo-nodes-py=0.14.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 20:11:07 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6350e2bac55c944dd34bc29e73fbc018fec2cf5e94689af115f8f54b5fec657b`  
		Last Modified: Fri, 09 Dec 2022 03:26:59 GMT  
		Size: 67.6 MB (67619151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a7b4cc4ed2f5afbc7072d331d05a7d4434dfabbef418886de0d8eb7de662f1`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 286.4 KB (286436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3991e0369f7386b610317863996480f39b063fff1a1b32babcb037cf7643a7`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345475a6e74d5f984d572de5f7122f7bad7e4b7a22e9914852dc4297ce04929f`  
		Last Modified: Fri, 09 Dec 2022 03:26:54 GMT  
		Size: 21.5 MB (21474900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488454374fa2fe150b42b83e6bd323fc2d0c53a6d6bb87c1727ee819bc5f9591`  
		Last Modified: Fri, 09 Dec 2022 03:27:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba85b3164e0b14e7381b4cfafd27fc1823b006f8d968497ae42a47b04edf356f`  
		Last Modified: Fri, 09 Dec 2022 03:27:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03429fd2aeb28001fc4c20d7f1d85a86731c83b0cf5eec280852a0122cd8a06`  
		Last Modified: Fri, 09 Dec 2022 03:27:27 GMT  
		Size: 78.7 MB (78668231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5c8c6be245a66da8bbe12873e21347a90c5888804f011355a3f09daa53c729`  
		Last Modified: Mon, 12 Dec 2022 20:12:33 GMT  
		Size: 16.0 MB (16012302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b097114b650bca3fb954ab6d8e4686c028944ceadb543b144e5b1845432e6f`  
		Last Modified: Mon, 12 Dec 2022 20:12:31 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:54f193b88f9efbd93a8281d7631c8ca87a1c3bc0c7274b6b63ed5805f5bccac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:951b800e7f0881c6436ef345689ac2f1da9750afaaca8f00fbd773b02fef3275
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330100546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e657f26897db359d6ce72d70068770a0a3eebb04a19d7bca0ad845929a9dd61`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:09:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:09:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:09:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:12:14 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 05:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:00 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:13:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:13:00 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:13:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:13:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 05:13:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:13:53 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 05:13:53 GMT
ENV ROS2_DISTRO=galactic
# Fri, 09 Dec 2022 05:14:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 21:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.4-1*     ros-galactic-demo-nodes-py=0.14.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 21:12:34 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd4df45a001dd08380ae069a426a705c7c8d6b3256c3d95bb0a8d281ea42c5`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb7876e8dbcfdfed9f4a879aa88de1c4785e20cbecb204dcccec3bfd76fa19a`  
		Last Modified: Fri, 09 Dec 2022 05:36:55 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad05d25a37392d09309c13d7f82f7882fcca6a1229113c9f96796b8f2b0a12`  
		Last Modified: Fri, 09 Dec 2022 05:38:26 GMT  
		Size: 103.9 MB (103902751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d26f18a583aa424d1037137f835a44ea407d294dfb4a483e4cbb250325f358`  
		Last Modified: Fri, 09 Dec 2022 05:38:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cb9e3c282d37d8c15c88800d126b8e236c391f7580ae4075c9eb1af48cd2be`  
		Last Modified: Fri, 09 Dec 2022 05:38:45 GMT  
		Size: 73.3 MB (73282784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def0d48a89f17574beb102c43e3542f8835cfcf9f91ceca92952f442cf8494b8`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 286.4 KB (286430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4223ffc392fc5e9b4afd8b6613332f44d08db8721ace9f392d0ab22e7a1b1a0`  
		Last Modified: Fri, 09 Dec 2022 05:38:34 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985a64d72dd41c16338473f48d90cbc5a2c63414c9e533bf85d8644dc78a57f`  
		Last Modified: Fri, 09 Dec 2022 05:38:38 GMT  
		Size: 22.1 MB (22138677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a516984ebca41375d3fdc82de7f43b9d8565c16de9d1e92073a45ec5e4de152`  
		Last Modified: Fri, 09 Dec 2022 05:38:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8344261bd56aeff273ec59554955f180c54c8a91313cac7b19b85ac1da1e9849`  
		Last Modified: Fri, 09 Dec 2022 05:38:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3d8a6822222d0f78e01589432f4fd8704e8419dae46b19c8b7121212bd369b`  
		Last Modified: Fri, 09 Dec 2022 05:39:10 GMT  
		Size: 78.7 MB (78709342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbf627443c5d8d8f5d4da4951347df2b77406e2292b0269de43b33fedc0471`  
		Last Modified: Mon, 12 Dec 2022 21:13:58 GMT  
		Size: 16.5 MB (16491975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca66a22ff38141d8f6ae0c4bf96c37d5424b1520b7b4b7a309e98e7a3669826`  
		Last Modified: Mon, 12 Dec 2022 21:13:55 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:01866ba9e9b22b8afe18221e789b3d0f4b90bf42400d29b928ede1afe6d3e417
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318266148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7646a811d85b21b2ba5e1c69cc35e79bc54d4a3b6ebb15bccefd852a34dbab97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:57:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 02:57:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:57:16 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:59:33 GMT
ENV ROS_DISTRO=galactic
# Fri, 09 Dec 2022 03:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:00:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:00:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:00:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:00:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:00:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 03:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:00:55 GMT
ENV ROS1_DISTRO=noetic
# Fri, 09 Dec 2022 03:00:55 GMT
ENV ROS2_DISTRO=galactic
# Fri, 09 Dec 2022 03:01:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 20:11:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.4-1*     ros-galactic-demo-nodes-py=0.14.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 12 Dec 2022 20:11:07 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a3301718be783bb7d10549e4c4d30d28c3440d4dd0dfc0e601d5c9ae213ab1`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63004661e39c1b539112611581f6e362b812038b6961c98254dd8ab0bb221832`  
		Last Modified: Fri, 09 Dec 2022 03:25:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18246af67f9bcf5f95f78e8287c9bb609ef2494bb98de3a9743f7b73e81c64e`  
		Last Modified: Fri, 09 Dec 2022 03:26:41 GMT  
		Size: 100.3 MB (100320700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdf1bae4bbb75b2d814386452fe8e42d53abb2be5ea3008b78a8307921829a`  
		Last Modified: Fri, 09 Dec 2022 03:26:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6350e2bac55c944dd34bc29e73fbc018fec2cf5e94689af115f8f54b5fec657b`  
		Last Modified: Fri, 09 Dec 2022 03:26:59 GMT  
		Size: 67.6 MB (67619151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a7b4cc4ed2f5afbc7072d331d05a7d4434dfabbef418886de0d8eb7de662f1`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 286.4 KB (286436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3991e0369f7386b610317863996480f39b063fff1a1b32babcb037cf7643a7`  
		Last Modified: Fri, 09 Dec 2022 03:26:51 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345475a6e74d5f984d572de5f7122f7bad7e4b7a22e9914852dc4297ce04929f`  
		Last Modified: Fri, 09 Dec 2022 03:26:54 GMT  
		Size: 21.5 MB (21474900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488454374fa2fe150b42b83e6bd323fc2d0c53a6d6bb87c1727ee819bc5f9591`  
		Last Modified: Fri, 09 Dec 2022 03:27:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba85b3164e0b14e7381b4cfafd27fc1823b006f8d968497ae42a47b04edf356f`  
		Last Modified: Fri, 09 Dec 2022 03:27:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03429fd2aeb28001fc4c20d7f1d85a86731c83b0cf5eec280852a0122cd8a06`  
		Last Modified: Fri, 09 Dec 2022 03:27:27 GMT  
		Size: 78.7 MB (78668231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5c8c6be245a66da8bbe12873e21347a90c5888804f011355a3f09daa53c729`  
		Last Modified: Mon, 12 Dec 2022 20:12:33 GMT  
		Size: 16.0 MB (16012302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b097114b650bca3fb954ab6d8e4686c028944ceadb543b144e5b1845432e6f`  
		Last Modified: Mon, 12 Dec 2022 20:12:31 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:187938e57357e2e1180ada88ddeb89bd54c156e444d09a1d92442c804c1cdf96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:31bef51bf3eebed981fb18f97475d3539a3c33192816f7d402b5490881e8bae9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263008434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff722dedce2c8b357f4a427a96c22a1317429723cda89e895aed0c58a3077074`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:17:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:17:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:17:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed26a8f7f4e4d3e8966acc0757bb9d7bbb705717c8d7196babebd7b5ff08f9`  
		Last Modified: Fri, 09 Dec 2022 05:39:59 GMT  
		Size: 97.9 MB (97882348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20036a4f3522ebf50ed296548e96acfd1c2ee142815c4f42a1f5920a1093ac03`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 306.0 KB (306038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f57b081e57005e855e03df50d834ac8a63a802e0687f87a62ad2222fe67e11`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de92fd9605557bfd0fe41102718c970ab0870f1c631991452d05dd06041d8b`  
		Last Modified: Fri, 09 Dec 2022 05:39:49 GMT  
		Size: 23.1 MB (23067539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:481ee52580335e2a6522cf3fc6240bfedecd0c0dfbe159604a7763f3858d8ac8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50155037927c12e45055330c93f9e104b2532ff6bae8dd7240415d4febfa3867`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:05:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:05:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:05:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d81ba9fa2ac44c9c12606bf311c5df2b8c1df0c6854c296d82c8cb9f3b202`  
		Last Modified: Fri, 09 Dec 2022 03:28:13 GMT  
		Size: 95.5 MB (95470615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac12414207ace7c477729fa77299c91bb8978e96da5cc581eb73e5c300b2b584`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 306.0 KB (306034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36392dab08181ad6041a8251345eabcd747f900681d10510fc8f9140e61f56bf`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 2.4 KB (2415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694dd25432411562e9e76144887e9e2160d41351325848671e4464c16c57960`  
		Last Modified: Fri, 09 Dec 2022 03:28:05 GMT  
		Size: 22.5 MB (22492246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:1ebf97c15fd45294f121ae4b7137ebc449d7308e4f656fab4afdb908df0d7c6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:dee7f8de7713abb581224d04e37538b0df1fc802f012d853f5b53f4f8952f609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1087296653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8730819807f2ca4cb7a9bef9a8494287a8866f8943f3fd2711978544066e684c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:17:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:17:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:17:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed26a8f7f4e4d3e8966acc0757bb9d7bbb705717c8d7196babebd7b5ff08f9`  
		Last Modified: Fri, 09 Dec 2022 05:39:59 GMT  
		Size: 97.9 MB (97882348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20036a4f3522ebf50ed296548e96acfd1c2ee142815c4f42a1f5920a1093ac03`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 306.0 KB (306038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f57b081e57005e855e03df50d834ac8a63a802e0687f87a62ad2222fe67e11`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de92fd9605557bfd0fe41102718c970ab0870f1c631991452d05dd06041d8b`  
		Last Modified: Fri, 09 Dec 2022 05:39:49 GMT  
		Size: 23.1 MB (23067539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77396d594b91eee162d53cfe75987e4a5a192f340d8868ea15f137239061aceb`  
		Last Modified: Fri, 09 Dec 2022 05:41:49 GMT  
		Size: 824.3 MB (824288219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5adfc6f63ae7422664dcc77d1c46e8e3336cb142a50cee574f1aaaada8de277f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1037577664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ebd5c570c2698230491c38e705d033238d6259a88b4c107721835dbebfbadf7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:05:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:05:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:05:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:16:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d81ba9fa2ac44c9c12606bf311c5df2b8c1df0c6854c296d82c8cb9f3b202`  
		Last Modified: Fri, 09 Dec 2022 03:28:13 GMT  
		Size: 95.5 MB (95470615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac12414207ace7c477729fa77299c91bb8978e96da5cc581eb73e5c300b2b584`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 306.0 KB (306034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36392dab08181ad6041a8251345eabcd747f900681d10510fc8f9140e61f56bf`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 2.4 KB (2415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694dd25432411562e9e76144887e9e2160d41351325848671e4464c16c57960`  
		Last Modified: Fri, 09 Dec 2022 03:28:05 GMT  
		Size: 22.5 MB (22492246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e237e5e98050952834a63108508af18dc56f80e79f151d6e23365c99a55e22`  
		Last Modified: Fri, 09 Dec 2022 03:29:47 GMT  
		Size: 781.9 MB (781892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:1ebf97c15fd45294f121ae4b7137ebc449d7308e4f656fab4afdb908df0d7c6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:dee7f8de7713abb581224d04e37538b0df1fc802f012d853f5b53f4f8952f609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1087296653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8730819807f2ca4cb7a9bef9a8494287a8866f8943f3fd2711978544066e684c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:17:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:17:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:17:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed26a8f7f4e4d3e8966acc0757bb9d7bbb705717c8d7196babebd7b5ff08f9`  
		Last Modified: Fri, 09 Dec 2022 05:39:59 GMT  
		Size: 97.9 MB (97882348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20036a4f3522ebf50ed296548e96acfd1c2ee142815c4f42a1f5920a1093ac03`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 306.0 KB (306038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f57b081e57005e855e03df50d834ac8a63a802e0687f87a62ad2222fe67e11`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de92fd9605557bfd0fe41102718c970ab0870f1c631991452d05dd06041d8b`  
		Last Modified: Fri, 09 Dec 2022 05:39:49 GMT  
		Size: 23.1 MB (23067539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77396d594b91eee162d53cfe75987e4a5a192f340d8868ea15f137239061aceb`  
		Last Modified: Fri, 09 Dec 2022 05:41:49 GMT  
		Size: 824.3 MB (824288219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5adfc6f63ae7422664dcc77d1c46e8e3336cb142a50cee574f1aaaada8de277f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1037577664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ebd5c570c2698230491c38e705d033238d6259a88b4c107721835dbebfbadf7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:05:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:05:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:05:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:16:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d81ba9fa2ac44c9c12606bf311c5df2b8c1df0c6854c296d82c8cb9f3b202`  
		Last Modified: Fri, 09 Dec 2022 03:28:13 GMT  
		Size: 95.5 MB (95470615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac12414207ace7c477729fa77299c91bb8978e96da5cc581eb73e5c300b2b584`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 306.0 KB (306034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36392dab08181ad6041a8251345eabcd747f900681d10510fc8f9140e61f56bf`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 2.4 KB (2415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694dd25432411562e9e76144887e9e2160d41351325848671e4464c16c57960`  
		Last Modified: Fri, 09 Dec 2022 03:28:05 GMT  
		Size: 22.5 MB (22492246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e237e5e98050952834a63108508af18dc56f80e79f151d6e23365c99a55e22`  
		Last Modified: Fri, 09 Dec 2022 03:29:47 GMT  
		Size: 781.9 MB (781892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:187938e57357e2e1180ada88ddeb89bd54c156e444d09a1d92442c804c1cdf96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:31bef51bf3eebed981fb18f97475d3539a3c33192816f7d402b5490881e8bae9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263008434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff722dedce2c8b357f4a427a96c22a1317429723cda89e895aed0c58a3077074`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:17:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:17:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:17:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed26a8f7f4e4d3e8966acc0757bb9d7bbb705717c8d7196babebd7b5ff08f9`  
		Last Modified: Fri, 09 Dec 2022 05:39:59 GMT  
		Size: 97.9 MB (97882348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20036a4f3522ebf50ed296548e96acfd1c2ee142815c4f42a1f5920a1093ac03`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 306.0 KB (306038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f57b081e57005e855e03df50d834ac8a63a802e0687f87a62ad2222fe67e11`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de92fd9605557bfd0fe41102718c970ab0870f1c631991452d05dd06041d8b`  
		Last Modified: Fri, 09 Dec 2022 05:39:49 GMT  
		Size: 23.1 MB (23067539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:481ee52580335e2a6522cf3fc6240bfedecd0c0dfbe159604a7763f3858d8ac8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50155037927c12e45055330c93f9e104b2532ff6bae8dd7240415d4febfa3867`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:05:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:05:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:05:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d81ba9fa2ac44c9c12606bf311c5df2b8c1df0c6854c296d82c8cb9f3b202`  
		Last Modified: Fri, 09 Dec 2022 03:28:13 GMT  
		Size: 95.5 MB (95470615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac12414207ace7c477729fa77299c91bb8978e96da5cc581eb73e5c300b2b584`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 306.0 KB (306034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36392dab08181ad6041a8251345eabcd747f900681d10510fc8f9140e61f56bf`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 2.4 KB (2415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694dd25432411562e9e76144887e9e2160d41351325848671e4464c16c57960`  
		Last Modified: Fri, 09 Dec 2022 03:28:05 GMT  
		Size: 22.5 MB (22492246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:187938e57357e2e1180ada88ddeb89bd54c156e444d09a1d92442c804c1cdf96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:31bef51bf3eebed981fb18f97475d3539a3c33192816f7d402b5490881e8bae9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263008434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff722dedce2c8b357f4a427a96c22a1317429723cda89e895aed0c58a3077074`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:17:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:17:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:17:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed26a8f7f4e4d3e8966acc0757bb9d7bbb705717c8d7196babebd7b5ff08f9`  
		Last Modified: Fri, 09 Dec 2022 05:39:59 GMT  
		Size: 97.9 MB (97882348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20036a4f3522ebf50ed296548e96acfd1c2ee142815c4f42a1f5920a1093ac03`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 306.0 KB (306038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f57b081e57005e855e03df50d834ac8a63a802e0687f87a62ad2222fe67e11`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de92fd9605557bfd0fe41102718c970ab0870f1c631991452d05dd06041d8b`  
		Last Modified: Fri, 09 Dec 2022 05:39:49 GMT  
		Size: 23.1 MB (23067539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:481ee52580335e2a6522cf3fc6240bfedecd0c0dfbe159604a7763f3858d8ac8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50155037927c12e45055330c93f9e104b2532ff6bae8dd7240415d4febfa3867`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:05:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:05:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:05:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d81ba9fa2ac44c9c12606bf311c5df2b8c1df0c6854c296d82c8cb9f3b202`  
		Last Modified: Fri, 09 Dec 2022 03:28:13 GMT  
		Size: 95.5 MB (95470615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac12414207ace7c477729fa77299c91bb8978e96da5cc581eb73e5c300b2b584`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 306.0 KB (306034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36392dab08181ad6041a8251345eabcd747f900681d10510fc8f9140e61f56bf`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 2.4 KB (2415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694dd25432411562e9e76144887e9e2160d41351325848671e4464c16c57960`  
		Last Modified: Fri, 09 Dec 2022 03:28:05 GMT  
		Size: 22.5 MB (22492246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:23aa104a31990bb6952f2836cbf431535ae53490d587a70b32e0ed94a9a4fd83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:de5d3049dbd0475512df89d3aca2e88ef62f642e5634575845ef21b85698d2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141750062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408ca0d60059d223feb3bdf8d9529a63f291b8978cd8437b1ac1acfaf33b5aac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:521bf25c64de69390b94dda61015087f28cb9eb59bcc383583e5d2a6bf04d98d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137414187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3e46567e32beaf8a4d507f7dfb0508872a826a4bf97b3fc929d497bbb8029`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:23aa104a31990bb6952f2836cbf431535ae53490d587a70b32e0ed94a9a4fd83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:de5d3049dbd0475512df89d3aca2e88ef62f642e5634575845ef21b85698d2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141750062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408ca0d60059d223feb3bdf8d9529a63f291b8978cd8437b1ac1acfaf33b5aac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:521bf25c64de69390b94dda61015087f28cb9eb59bcc383583e5d2a6bf04d98d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137414187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3e46567e32beaf8a4d507f7dfb0508872a826a4bf97b3fc929d497bbb8029`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:187938e57357e2e1180ada88ddeb89bd54c156e444d09a1d92442c804c1cdf96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:31bef51bf3eebed981fb18f97475d3539a3c33192816f7d402b5490881e8bae9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263008434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff722dedce2c8b357f4a427a96c22a1317429723cda89e895aed0c58a3077074`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 05:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:16:43 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:16:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:16:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:17:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:17:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:17:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f1ebc7554e42ae1b84803d3582ff0d979e2cae57350f8fa7c7f19d10af22d`  
		Last Modified: Fri, 09 Dec 2022 05:39:36 GMT  
		Size: 106.3 MB (106322004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8e7fea243b895feae68411ade9458a3b0c035e1043382c93036a12b1fab7a`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed26a8f7f4e4d3e8966acc0757bb9d7bbb705717c8d7196babebd7b5ff08f9`  
		Last Modified: Fri, 09 Dec 2022 05:39:59 GMT  
		Size: 97.9 MB (97882348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20036a4f3522ebf50ed296548e96acfd1c2ee142815c4f42a1f5920a1093ac03`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 306.0 KB (306038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f57b081e57005e855e03df50d834ac8a63a802e0687f87a62ad2222fe67e11`  
		Last Modified: Fri, 09 Dec 2022 05:39:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de92fd9605557bfd0fe41102718c970ab0870f1c631991452d05dd06041d8b`  
		Last Modified: Fri, 09 Dec 2022 05:39:49 GMT  
		Size: 23.1 MB (23067539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:481ee52580335e2a6522cf3fc6240bfedecd0c0dfbe159604a7763f3858d8ac8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255685497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50155037927c12e45055330c93f9e104b2532ff6bae8dd7240415d4febfa3867`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV ROS_DISTRO=humble
# Fri, 09 Dec 2022 03:04:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:04:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:04:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:04:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:05:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:05:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:05:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c663a312d54a8bf361593f850418988d836fd90bae2c046888143349e739d90`  
		Last Modified: Fri, 09 Dec 2022 03:27:53 GMT  
		Size: 104.1 MB (104055235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c207355d120614d12bc04f3a3395974c224633425e14ee694502a70b394ff9f5`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d81ba9fa2ac44c9c12606bf311c5df2b8c1df0c6854c296d82c8cb9f3b202`  
		Last Modified: Fri, 09 Dec 2022 03:28:13 GMT  
		Size: 95.5 MB (95470615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac12414207ace7c477729fa77299c91bb8978e96da5cc581eb73e5c300b2b584`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 306.0 KB (306034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36392dab08181ad6041a8251345eabcd747f900681d10510fc8f9140e61f56bf`  
		Last Modified: Fri, 09 Dec 2022 03:28:01 GMT  
		Size: 2.4 KB (2415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694dd25432411562e9e76144887e9e2160d41351325848671e4464c16c57960`  
		Last Modified: Fri, 09 Dec 2022 03:28:05 GMT  
		Size: 22.5 MB (22492246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:8826c838aa7c8022aaeebefb0780e7d07d8990b3b0883fdb787ff1853581e79d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:9537ef66aeb589fabe2107801800f0dcdab9ab262e05d26083483abc9ddf7a42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437537690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4b0e72e44d75f8238ec2e654658dcc36aeba42d1f33229a2c01c734735df5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f939ad9f1402b712bc6a412ca4d73e1b59e3cdb078ba847dfda37d6a0905c4c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386013747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ad9626d781dcd3eed605a18a27474241a346cc639ec742779184dc327f708c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6ca358e86ac9739a9a2b0f6e1dd7cd081d8c5583fed52fa33de61cd5561b2745
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412178550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe318468fc432b0392e3733f37fabe417080ce4e50304811b84a2c79a9eff996`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:6e53e928710fb72695eea62704308722213a91119666ce718bd58613abd00fb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:83c6b74745cc2c5775bc3f26d7311a5f6ca38c02c0abd8ff26bd9d1083ea0968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742902932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c46af7c2a81303ec6450990be4dcbe31748df7b0823b41fd930c1704cdbd6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2875b4dae8dac43004d9842f3b9276123c21c20a852cd6ae98172199c9f1877`  
		Last Modified: Fri, 09 Dec 2022 05:34:09 GMT  
		Size: 305.4 MB (305365242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:3e6fadd5e021e9b3b6f0d2cf2c598ee29f4fde3346977547879ed5b2e867679b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (646048525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c88596513df9786719f2880d4fcfe5c83f8a581073cb8f567a7402b2ceaedab`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:09:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40813fa40c887843e03c03395b27ef55a365e8f170a58fcb5aa2b3a31d4be4d2`  
		Last Modified: Fri, 09 Dec 2022 02:28:37 GMT  
		Size: 260.0 MB (260034778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bbf2a89595c6b092c33478bdc52ac166ef0e9c62ef3d5143bc958e4df49f93d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.9 MB (703863322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91805d98b3c3eb69af39cc8090656300774d9a82ff6b81af9ba912ef141eec94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c45d501b8dda7ced18a53eca302aac95ad0c62ff20d9e381cc5c7b19b45372`  
		Last Modified: Fri, 09 Dec 2022 03:22:48 GMT  
		Size: 291.7 MB (291684772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:6e53e928710fb72695eea62704308722213a91119666ce718bd58613abd00fb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:83c6b74745cc2c5775bc3f26d7311a5f6ca38c02c0abd8ff26bd9d1083ea0968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742902932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c46af7c2a81303ec6450990be4dcbe31748df7b0823b41fd930c1704cdbd6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:55:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2875b4dae8dac43004d9842f3b9276123c21c20a852cd6ae98172199c9f1877`  
		Last Modified: Fri, 09 Dec 2022 05:34:09 GMT  
		Size: 305.4 MB (305365242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3e6fadd5e021e9b3b6f0d2cf2c598ee29f4fde3346977547879ed5b2e867679b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (646048525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c88596513df9786719f2880d4fcfe5c83f8a581073cb8f567a7402b2ceaedab`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:09:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40813fa40c887843e03c03395b27ef55a365e8f170a58fcb5aa2b3a31d4be4d2`  
		Last Modified: Fri, 09 Dec 2022 02:28:37 GMT  
		Size: 260.0 MB (260034778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bbf2a89595c6b092c33478bdc52ac166ef0e9c62ef3d5143bc958e4df49f93d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.9 MB (703863322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91805d98b3c3eb69af39cc8090656300774d9a82ff6b81af9ba912ef141eec94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c45d501b8dda7ced18a53eca302aac95ad0c62ff20d9e381cc5c7b19b45372`  
		Last Modified: Fri, 09 Dec 2022 03:22:48 GMT  
		Size: 291.7 MB (291684772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:7299ad118aeb48ffdd1977632807665a5f5179bbc254e52c7167f55b2fe83c92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:36219518431cab7236a5bda7f1b2b7a96213a1c6f3ad238a54d3f2d37dcefdd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448623580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27c3e8b5aef7bddcbfae97d6c436331623e7ec7a0660d90a8276c9645877a95`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:50:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64ab5304617ee2844cf855044219cb3be917ff41ceed7efa040a50b1b7efd43`  
		Last Modified: Fri, 09 Dec 2022 05:33:13 GMT  
		Size: 11.1 MB (11085890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:fd73a5a9f6d7c6d251fc7fe60e04a2191b38c3e1851e01c1b4c922853d4efdda
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396136208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bbf4f6a04779179625f24a235ae9f6a29712be155da6285d6f82c0a493bdf6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:03:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ee2fec37f55b2a63082f6cee34bab8f62cb1e6e8ac12b4d3cfa7c4de883984`  
		Last Modified: Fri, 09 Dec 2022 02:27:42 GMT  
		Size: 10.1 MB (10122461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:72f6ab715c4af1a3320128ce3b1c059ea88093cf278e62902b98c0e6720543b4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422918108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb723ef47d7779547ceeae1a1b1db06fe95bc356910456181e45b4ed49afc11`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:37:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8fb080e70ce7bac2b65be37886f40542b51fdf0171694b3773f20f5bb51b66`  
		Last Modified: Fri, 09 Dec 2022 03:22:01 GMT  
		Size: 10.7 MB (10739558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:7299ad118aeb48ffdd1977632807665a5f5179bbc254e52c7167f55b2fe83c92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:36219518431cab7236a5bda7f1b2b7a96213a1c6f3ad238a54d3f2d37dcefdd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448623580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27c3e8b5aef7bddcbfae97d6c436331623e7ec7a0660d90a8276c9645877a95`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:50:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64ab5304617ee2844cf855044219cb3be917ff41ceed7efa040a50b1b7efd43`  
		Last Modified: Fri, 09 Dec 2022 05:33:13 GMT  
		Size: 11.1 MB (11085890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:fd73a5a9f6d7c6d251fc7fe60e04a2191b38c3e1851e01c1b4c922853d4efdda
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396136208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bbf4f6a04779179625f24a235ae9f6a29712be155da6285d6f82c0a493bdf6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:03:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ee2fec37f55b2a63082f6cee34bab8f62cb1e6e8ac12b4d3cfa7c4de883984`  
		Last Modified: Fri, 09 Dec 2022 02:27:42 GMT  
		Size: 10.1 MB (10122461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:72f6ab715c4af1a3320128ce3b1c059ea88093cf278e62902b98c0e6720543b4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422918108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb723ef47d7779547ceeae1a1b1db06fe95bc356910456181e45b4ed49afc11`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:37:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8fb080e70ce7bac2b65be37886f40542b51fdf0171694b3773f20f5bb51b66`  
		Last Modified: Fri, 09 Dec 2022 03:22:01 GMT  
		Size: 10.7 MB (10739558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:8826c838aa7c8022aaeebefb0780e7d07d8990b3b0883fdb787ff1853581e79d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:9537ef66aeb589fabe2107801800f0dcdab9ab262e05d26083483abc9ddf7a42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437537690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4b0e72e44d75f8238ec2e654658dcc36aeba42d1f33229a2c01c734735df5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:f939ad9f1402b712bc6a412ca4d73e1b59e3cdb078ba847dfda37d6a0905c4c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386013747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ad9626d781dcd3eed605a18a27474241a346cc639ec742779184dc327f708c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6ca358e86ac9739a9a2b0f6e1dd7cd081d8c5583fed52fa33de61cd5561b2745
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412178550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe318468fc432b0392e3733f37fabe417080ce4e50304811b84a2c79a9eff996`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:8826c838aa7c8022aaeebefb0780e7d07d8990b3b0883fdb787ff1853581e79d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:9537ef66aeb589fabe2107801800f0dcdab9ab262e05d26083483abc9ddf7a42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437537690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4b0e72e44d75f8238ec2e654658dcc36aeba42d1f33229a2c01c734735df5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:48:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:48:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 04:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b499e7744ee3ef3342ad829a9c9fba7aca4d39a81dcb389a6d2f45dac023f0a`  
		Last Modified: Fri, 09 Dec 2022 05:32:59 GMT  
		Size: 70.3 MB (70260139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148224ce393ec2998511d1982fa48ecd1c5f046d78a7632b77a1c56ad0dd48c2`  
		Last Modified: Fri, 09 Dec 2022 05:32:49 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2964397cdd41f429498d2c9abc9969c85476bb883029783a17298f819f4dbe0b`  
		Last Modified: Fri, 09 Dec 2022 05:33:01 GMT  
		Size: 75.0 MB (75000867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f939ad9f1402b712bc6a412ca4d73e1b59e3cdb078ba847dfda37d6a0905c4c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386013747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ad9626d781dcd3eed605a18a27474241a346cc639ec742779184dc327f708c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:01:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:02:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd36127e353e3165e87518700719f715f7dc291ab1f13092b0d0f60cc3d2d`  
		Last Modified: Fri, 09 Dec 2022 02:27:20 GMT  
		Size: 54.7 MB (54722170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7191f0e58d67f8750b2a4f4ad1ec8da5a15636427e70f7e9a31d9b577360eb`  
		Last Modified: Fri, 09 Dec 2022 02:27:11 GMT  
		Size: 294.9 KB (294881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c47dc5d23a8092314cfe45f481ce0c5f5972e63796944db46f95e82183c6c9`  
		Last Modified: Fri, 09 Dec 2022 02:27:23 GMT  
		Size: 64.7 MB (64749165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6ca358e86ac9739a9a2b0f6e1dd7cd081d8c5583fed52fa33de61cd5561b2745
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412178550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe318468fc432b0392e3733f37fabe417080ce4e50304811b84a2c79a9eff996`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:35:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:35:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb05a26fe43b56bbc6fecdec3bf5d53028ce867e0a0a1eb22d78d2f40db24`  
		Last Modified: Fri, 09 Dec 2022 03:21:45 GMT  
		Size: 63.1 MB (63090368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d0b2a0df05f016d80d36dffa018b041ea6deeb604b49565fb07423fe8538ea`  
		Last Modified: Fri, 09 Dec 2022 03:21:38 GMT  
		Size: 294.9 KB (294898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e36e48a632f552219edbe4a578063e34ee68d11178b09d7dd5604138899fdf`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 67.2 MB (67234776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:a3b125e1c3878c6b9a9a1fffeeb501440fc8aa95b9fe55e4747857190c2720e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:e63efc8d3dcc12b35471b985ae23584e5f60842f5a91cd2adbdf8b9794e597c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291981786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e529341f61d8acdd4d6a5ee0b19a927dca4ccddc8ff3b18c0a26f4e914a1c18e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5c912d5c5ba14503727abe4ad8027257d321d59b78fd4eca576f9ffaea9e8deb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266247531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d74b49e7f558f88a94a3d8e4940d4e66a40c3139700cce81c1206f67a574ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4761e3a78091f3a3b115082988e372ace4f03ae30b7d2d81650f85ec3bc0a8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281558508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779f48d9a3dd10268a4144638379699a2ae7d0eddb22efdd72b7f4cb1a0108e1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:a3b125e1c3878c6b9a9a1fffeeb501440fc8aa95b9fe55e4747857190c2720e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:e63efc8d3dcc12b35471b985ae23584e5f60842f5a91cd2adbdf8b9794e597c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291981786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e529341f61d8acdd4d6a5ee0b19a927dca4ccddc8ff3b18c0a26f4e914a1c18e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:5c912d5c5ba14503727abe4ad8027257d321d59b78fd4eca576f9ffaea9e8deb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266247531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d74b49e7f558f88a94a3d8e4940d4e66a40c3139700cce81c1206f67a574ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4761e3a78091f3a3b115082988e372ace4f03ae30b7d2d81650f85ec3bc0a8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281558508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779f48d9a3dd10268a4144638379699a2ae7d0eddb22efdd72b7f4cb1a0108e1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:05aab2a99ce2a82114702ab96fad303931550f526d653ac46fc77160e779f287
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:a6d60e329c918cf340858effdd28e13d66a6bf0541b96e647242de597a386732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343186980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4431c3220c78f40fafe49622a3d2e51646341b4ac86ea5ad573e7c67e4c3e031`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:d17750dfa2dbd08fed5f26066b582ccf50451669e8978766e1cb48dd30391e6f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289283606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9be7b8f21dff9b49ad4024be643163437356117bb2dcebf68bea286629f273`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f91972d4c1b3993884e1b4bb6202bc010a485b216aafdf67f0b02061198b2cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322850055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6efff5e9eebc1d010289b96f74b9b3c5b0e5331af7d6cfe3031d5ca016959d42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:58a5e4ad3653a0172cddef33291208880846e308f6a57f888a7d69314963b3b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:13a262fe4ad9b7eecbf07f72d23bf6e3533f80f740db8119c60012489fd6578e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835158418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5eb91c9d23e4e2d7a025882ee7d889a3f99c2f1250de3d837d04b3b0adb79c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91b6364b9e818d3f74dc15ed73bb714a5bea9ab335cf0f3b4e2e85a1cb3c2cd`  
		Last Modified: Fri, 09 Dec 2022 05:36:43 GMT  
		Size: 492.0 MB (491971438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:520ff71d2a8a35cc0c565ff82fc564b58d13e7f5f099c0302b5243e95f447823
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726209263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d457b04355d08d9fa7ef46650e64d513dd3a5763ccfdd54823f95f7297fd189f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:25:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37339769e11ac31ece1d77df7f19d17aeb6624d5bd44589ca9a6374746db2f2f`  
		Last Modified: Fri, 09 Dec 2022 02:31:28 GMT  
		Size: 436.9 MB (436925657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed52e1bb062b123ab7c64f6ad962a25ab6e4c138337b707eab85cdc1525ef160
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785417179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1871809c1e31ff48cf9511a71cc2ef20040807731e7a205293035d00fcdeea5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:56:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d74ac54536fb2ed71dadda185aa38ce4d1a74891ed97ddffc772b9dd24eeba`  
		Last Modified: Fri, 09 Dec 2022 03:25:05 GMT  
		Size: 462.6 MB (462567124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:b917b8afa207e0932de817b5ed403cea0daa3a2edc3b494a08a941cf70680843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:118ea7c7ae6390acd2aded6d156de90bdd4ee8a4b1c6761db9477a6cc082a6cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.2 MB (951209677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20541cbb2cb1454e3836c081c246aaf6c41c38f9e0f5e43524b27652476bfa79`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:41 GMT
ADD file:c865da7afcf35b5a9538e63633f7e99ae4c40933cb8a0235e9704713042fba66 in / 
# Wed, 21 Dec 2022 01:20:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:00:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:00:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 11:00:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 11:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:01:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 11:01:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 11:01:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:02:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:02:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 11:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:07:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7c50787e2da71205402343dd1233b3ca6ebe70c7e790f6ba7d856b81b893200`  
		Last Modified: Wed, 21 Dec 2022 01:24:55 GMT  
		Size: 50.4 MB (50448893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b052e3063dd5e1f5dd43ac9327c08a1f0ba5c05673755f0ddbc54eb8a47b68ed`  
		Last Modified: Wed, 21 Dec 2022 11:08:36 GMT  
		Size: 10.9 MB (10896939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83902353ad66fb52936b96293c207b00d5b37b587f35948ca0a2e679a1f0a0e`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cadf3ead30322d6c27a63204270292209d103c528b40928749587f9d7e136a`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c16a3a9b3a8fe00067d85297c8380ad068e3b1f484b284f35f9d54feaa04d`  
		Last Modified: Wed, 21 Dec 2022 11:09:08 GMT  
		Size: 239.2 MB (239205442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9168ac3a9e93b34a9b55bbd10385b07a62b2e6d6cc2c2ea2fde52bae7aeb96`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574b7ce55ba7fdaaeec166ec647f6340cc91a1a2e51d56611321212e582fc441`  
		Last Modified: Wed, 21 Dec 2022 11:09:30 GMT  
		Size: 86.6 MB (86603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e570d3835677549b55dae60d3bde8885640704299063b3c01e2f7fcb51c7ba`  
		Last Modified: Wed, 21 Dec 2022 11:09:17 GMT  
		Size: 334.8 KB (334763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42887f47d573625da7116cd5dd3aac01fdd922e84fb04cb757dc6f62ae7637fa`  
		Last Modified: Wed, 21 Dec 2022 11:09:28 GMT  
		Size: 76.0 MB (75978042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeebe1fcaed8ad561cfb4d7dd2eac4b207065e33f753942df31c82b82018cf5`  
		Last Modified: Wed, 21 Dec 2022 11:10:58 GMT  
		Size: 487.7 MB (487740170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:68148b43392cedc2ac5baeff8fbebfb5840ca68d43fa388b9170dbe8ae03b766
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.0 MB (868008808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa505f56ea448629dc64c0356a62615858454c77bc271486eda5250e49375fbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:12:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:12:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 12:12:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 12:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:13:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 12:13:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 12:13:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:14:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:14:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 12:15:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08619936cad6d315f51012474fa22f2fd8f1b475904aeeff8ab1ac9c94fb0770`  
		Last Modified: Wed, 21 Dec 2022 12:20:30 GMT  
		Size: 10.9 MB (10902542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49515cbca6d7dbd9df1f61795afce1f6540a7a7311f1e810e4e6119c9fe2b775`  
		Last Modified: Wed, 21 Dec 2022 12:20:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b1d3f149f7c168a510f4e797a86641439ab36f1672b64c32293d7f8c8501bc`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843956780ad36f94b7e0b598faa8c34f95b66ed491d15dc1b1d415e442f55810`  
		Last Modified: Wed, 21 Dec 2022 12:20:52 GMT  
		Size: 184.4 MB (184388328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689420f0e90e19012bdbc76769c6d25d3029bb1789f3f4e11b26ddfc71c98cb5`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cafe663c78ec8ec83680ea83b1eb1d875557336eaa0250b7da09cf2a31a73a9`  
		Last Modified: Wed, 21 Dec 2022 12:21:07 GMT  
		Size: 84.4 MB (84392573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed64ee0e529545d23cbf4774ca33327a650a6c43ac3538b89be5f1c573c6d3f`  
		Last Modified: Wed, 21 Dec 2022 12:20:58 GMT  
		Size: 334.8 KB (334765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bb1fb353f747aa2cdd4952aa366c48c03fd0a22dc2a88790e59ba8edd5c98d`  
		Last Modified: Wed, 21 Dec 2022 12:21:06 GMT  
		Size: 74.1 MB (74089601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c304188c356ac7ab29c9db8f7e634caeaf378e55c425f6044983ee201bdac1`  
		Last Modified: Wed, 21 Dec 2022 12:22:11 GMT  
		Size: 464.7 MB (464664770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:58a5e4ad3653a0172cddef33291208880846e308f6a57f888a7d69314963b3b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:13a262fe4ad9b7eecbf07f72d23bf6e3533f80f740db8119c60012489fd6578e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835158418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5eb91c9d23e4e2d7a025882ee7d889a3f99c2f1250de3d837d04b3b0adb79c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91b6364b9e818d3f74dc15ed73bb714a5bea9ab335cf0f3b4e2e85a1cb3c2cd`  
		Last Modified: Fri, 09 Dec 2022 05:36:43 GMT  
		Size: 492.0 MB (491971438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:520ff71d2a8a35cc0c565ff82fc564b58d13e7f5f099c0302b5243e95f447823
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726209263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d457b04355d08d9fa7ef46650e64d513dd3a5763ccfdd54823f95f7297fd189f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:25:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37339769e11ac31ece1d77df7f19d17aeb6624d5bd44589ca9a6374746db2f2f`  
		Last Modified: Fri, 09 Dec 2022 02:31:28 GMT  
		Size: 436.9 MB (436925657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed52e1bb062b123ab7c64f6ad962a25ab6e4c138337b707eab85cdc1525ef160
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785417179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1871809c1e31ff48cf9511a71cc2ef20040807731e7a205293035d00fcdeea5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:56:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d74ac54536fb2ed71dadda185aa38ce4d1a74891ed97ddffc772b9dd24eeba`  
		Last Modified: Fri, 09 Dec 2022 03:25:05 GMT  
		Size: 462.6 MB (462567124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:e778953aab40194b3c7a839dc6dca42023b338da8558ed2223e3c44d5b7d3d4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:4a867faa225107832dcbaf4f210beaa5229a4bcc336abe610f6726bbda4c2fba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359048413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63508127062f573c37425c58e540f921efc290d9976a6a02cce0ffcfb9cfcd0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75203dd5727607450789d9c86ce7b90133f512b8f2a7a39c19120bae4931f4c0`  
		Last Modified: Fri, 09 Dec 2022 05:35:22 GMT  
		Size: 15.9 MB (15861433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:f956e93ab3e441651029de6488a2f211fca560ca4461980e7ab44d9719faad01
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303352775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41bfdcfd1abdf0a65219142665077fef9720639a94b71cef480aef71ff7338d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:17:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f876436b511f8e7f61400d5abfb73b73dee9560a922a80dca1f666b7a8dca5b`  
		Last Modified: Fri, 09 Dec 2022 02:30:04 GMT  
		Size: 14.1 MB (14069169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:733437852e3d9b267e4cb0a721d6b8923d9ecf800aabd0310885adf118a7d205
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338303759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97943316580e70b670f1108be9026204396071e451d89e1aabb54e1e8c3652d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79075bc5b2a2e2ec7f838ff2c41866bc858d90f35ba8cb4dd3a83b3b1a73cb3`  
		Last Modified: Fri, 09 Dec 2022 03:23:59 GMT  
		Size: 15.5 MB (15453704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:b3e21be29ba770550632b2660e89eb534689f5719b99e464036351e15e68af26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:5a7f86c927079a5680dc6894240b166341ccd35b5e783083e83c065061eccc01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.6 MB (484624407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f97007696a1b2771f425f817c07e7a6f54a8200cde3fb9f660a51027e2ffdc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:41 GMT
ADD file:c865da7afcf35b5a9538e63633f7e99ae4c40933cb8a0235e9704713042fba66 in / 
# Wed, 21 Dec 2022 01:20:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:00:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:00:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 11:00:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 11:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:01:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 11:01:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 11:01:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:02:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:02:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 11:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:03:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7c50787e2da71205402343dd1233b3ca6ebe70c7e790f6ba7d856b81b893200`  
		Last Modified: Wed, 21 Dec 2022 01:24:55 GMT  
		Size: 50.4 MB (50448893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b052e3063dd5e1f5dd43ac9327c08a1f0ba5c05673755f0ddbc54eb8a47b68ed`  
		Last Modified: Wed, 21 Dec 2022 11:08:36 GMT  
		Size: 10.9 MB (10896939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83902353ad66fb52936b96293c207b00d5b37b587f35948ca0a2e679a1f0a0e`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cadf3ead30322d6c27a63204270292209d103c528b40928749587f9d7e136a`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c16a3a9b3a8fe00067d85297c8380ad068e3b1f484b284f35f9d54feaa04d`  
		Last Modified: Wed, 21 Dec 2022 11:09:08 GMT  
		Size: 239.2 MB (239205442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9168ac3a9e93b34a9b55bbd10385b07a62b2e6d6cc2c2ea2fde52bae7aeb96`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574b7ce55ba7fdaaeec166ec647f6340cc91a1a2e51d56611321212e582fc441`  
		Last Modified: Wed, 21 Dec 2022 11:09:30 GMT  
		Size: 86.6 MB (86603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e570d3835677549b55dae60d3bde8885640704299063b3c01e2f7fcb51c7ba`  
		Last Modified: Wed, 21 Dec 2022 11:09:17 GMT  
		Size: 334.8 KB (334763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42887f47d573625da7116cd5dd3aac01fdd922e84fb04cb757dc6f62ae7637fa`  
		Last Modified: Wed, 21 Dec 2022 11:09:28 GMT  
		Size: 76.0 MB (75978042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97947107aba0f0467ae57bae9eb05f15f95582dfc840921ade777ad411375019`  
		Last Modified: Wed, 21 Dec 2022 11:09:38 GMT  
		Size: 21.2 MB (21154900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:699858e1b85182436683b2629c4c430a40579f502d65c6b6df0cd78c5f8b14a8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424161781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:571dd4b77e50e35193ffe4f09ad47ef91b10f162a0ba98358a7ece34a35cbbb9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:12:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:12:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 12:12:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 12:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:13:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 12:13:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 12:13:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:14:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:14:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 12:15:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:15:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08619936cad6d315f51012474fa22f2fd8f1b475904aeeff8ab1ac9c94fb0770`  
		Last Modified: Wed, 21 Dec 2022 12:20:30 GMT  
		Size: 10.9 MB (10902542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49515cbca6d7dbd9df1f61795afce1f6540a7a7311f1e810e4e6119c9fe2b775`  
		Last Modified: Wed, 21 Dec 2022 12:20:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b1d3f149f7c168a510f4e797a86641439ab36f1672b64c32293d7f8c8501bc`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843956780ad36f94b7e0b598faa8c34f95b66ed491d15dc1b1d415e442f55810`  
		Last Modified: Wed, 21 Dec 2022 12:20:52 GMT  
		Size: 184.4 MB (184388328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689420f0e90e19012bdbc76769c6d25d3029bb1789f3f4e11b26ddfc71c98cb5`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cafe663c78ec8ec83680ea83b1eb1d875557336eaa0250b7da09cf2a31a73a9`  
		Last Modified: Wed, 21 Dec 2022 12:21:07 GMT  
		Size: 84.4 MB (84392573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed64ee0e529545d23cbf4774ca33327a650a6c43ac3538b89be5f1c573c6d3f`  
		Last Modified: Wed, 21 Dec 2022 12:20:58 GMT  
		Size: 334.8 KB (334765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bb1fb353f747aa2cdd4952aa366c48c03fd0a22dc2a88790e59ba8edd5c98d`  
		Last Modified: Wed, 21 Dec 2022 12:21:06 GMT  
		Size: 74.1 MB (74089601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f2ac528ed2ea48347b30f1fbcf4319d1c92f7e84aa5ae6c74bb78ed0bca7a0`  
		Last Modified: Wed, 21 Dec 2022 12:21:15 GMT  
		Size: 20.8 MB (20817743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:e778953aab40194b3c7a839dc6dca42023b338da8558ed2223e3c44d5b7d3d4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:4a867faa225107832dcbaf4f210beaa5229a4bcc336abe610f6726bbda4c2fba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359048413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63508127062f573c37425c58e540f921efc290d9976a6a02cce0ffcfb9cfcd0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75203dd5727607450789d9c86ce7b90133f512b8f2a7a39c19120bae4931f4c0`  
		Last Modified: Fri, 09 Dec 2022 05:35:22 GMT  
		Size: 15.9 MB (15861433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:f956e93ab3e441651029de6488a2f211fca560ca4461980e7ab44d9719faad01
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303352775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41bfdcfd1abdf0a65219142665077fef9720639a94b71cef480aef71ff7338d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:17:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f876436b511f8e7f61400d5abfb73b73dee9560a922a80dca1f666b7a8dca5b`  
		Last Modified: Fri, 09 Dec 2022 02:30:04 GMT  
		Size: 14.1 MB (14069169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:733437852e3d9b267e4cb0a721d6b8923d9ecf800aabd0310885adf118a7d205
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338303759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97943316580e70b670f1108be9026204396071e451d89e1aabb54e1e8c3652d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79075bc5b2a2e2ec7f838ff2c41866bc858d90f35ba8cb4dd3a83b3b1a73cb3`  
		Last Modified: Fri, 09 Dec 2022 03:23:59 GMT  
		Size: 15.5 MB (15453704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:05aab2a99ce2a82114702ab96fad303931550f526d653ac46fc77160e779f287
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a6d60e329c918cf340858effdd28e13d66a6bf0541b96e647242de597a386732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343186980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4431c3220c78f40fafe49622a3d2e51646341b4ac86ea5ad573e7c67e4c3e031`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:d17750dfa2dbd08fed5f26066b582ccf50451669e8978766e1cb48dd30391e6f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289283606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9be7b8f21dff9b49ad4024be643163437356117bb2dcebf68bea286629f273`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f91972d4c1b3993884e1b4bb6202bc010a485b216aafdf67f0b02061198b2cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322850055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6efff5e9eebc1d010289b96f74b9b3c5b0e5331af7d6cfe3031d5ca016959d42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:672ef48238a5e73b5645a94dd07512c01c3d3d9de669c823fa045039b26d24c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:e8a3701929befc990b68f6c83d0722142cb5d73da96b631e89913e2fa5b7e67f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.5 MB (463469507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267bb861abdc00137b346e85ad8d63656819fdfc4533df191a50f4f0225e2731`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:41 GMT
ADD file:c865da7afcf35b5a9538e63633f7e99ae4c40933cb8a0235e9704713042fba66 in / 
# Wed, 21 Dec 2022 01:20:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:00:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:00:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 11:00:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 11:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:01:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 11:01:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 11:01:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:02:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:02:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 11:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7c50787e2da71205402343dd1233b3ca6ebe70c7e790f6ba7d856b81b893200`  
		Last Modified: Wed, 21 Dec 2022 01:24:55 GMT  
		Size: 50.4 MB (50448893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b052e3063dd5e1f5dd43ac9327c08a1f0ba5c05673755f0ddbc54eb8a47b68ed`  
		Last Modified: Wed, 21 Dec 2022 11:08:36 GMT  
		Size: 10.9 MB (10896939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83902353ad66fb52936b96293c207b00d5b37b587f35948ca0a2e679a1f0a0e`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cadf3ead30322d6c27a63204270292209d103c528b40928749587f9d7e136a`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c16a3a9b3a8fe00067d85297c8380ad068e3b1f484b284f35f9d54feaa04d`  
		Last Modified: Wed, 21 Dec 2022 11:09:08 GMT  
		Size: 239.2 MB (239205442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9168ac3a9e93b34a9b55bbd10385b07a62b2e6d6cc2c2ea2fde52bae7aeb96`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574b7ce55ba7fdaaeec166ec647f6340cc91a1a2e51d56611321212e582fc441`  
		Last Modified: Wed, 21 Dec 2022 11:09:30 GMT  
		Size: 86.6 MB (86603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e570d3835677549b55dae60d3bde8885640704299063b3c01e2f7fcb51c7ba`  
		Last Modified: Wed, 21 Dec 2022 11:09:17 GMT  
		Size: 334.8 KB (334763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42887f47d573625da7116cd5dd3aac01fdd922e84fb04cb757dc6f62ae7637fa`  
		Last Modified: Wed, 21 Dec 2022 11:09:28 GMT  
		Size: 76.0 MB (75978042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b5e47a477b17a64bfd639b4cbfbc6680d565ef65b94c0f58b2da54a1a705d333
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403344038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ab8736ff086707bd8f2daf48be056d676d526b376527f860f8ddf2bc4d92de`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:12:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:12:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 12:12:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 12:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:13:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 12:13:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 12:13:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:14:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:14:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 12:15:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08619936cad6d315f51012474fa22f2fd8f1b475904aeeff8ab1ac9c94fb0770`  
		Last Modified: Wed, 21 Dec 2022 12:20:30 GMT  
		Size: 10.9 MB (10902542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49515cbca6d7dbd9df1f61795afce1f6540a7a7311f1e810e4e6119c9fe2b775`  
		Last Modified: Wed, 21 Dec 2022 12:20:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b1d3f149f7c168a510f4e797a86641439ab36f1672b64c32293d7f8c8501bc`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843956780ad36f94b7e0b598faa8c34f95b66ed491d15dc1b1d415e442f55810`  
		Last Modified: Wed, 21 Dec 2022 12:20:52 GMT  
		Size: 184.4 MB (184388328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689420f0e90e19012bdbc76769c6d25d3029bb1789f3f4e11b26ddfc71c98cb5`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cafe663c78ec8ec83680ea83b1eb1d875557336eaa0250b7da09cf2a31a73a9`  
		Last Modified: Wed, 21 Dec 2022 12:21:07 GMT  
		Size: 84.4 MB (84392573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed64ee0e529545d23cbf4774ca33327a650a6c43ac3538b89be5f1c573c6d3f`  
		Last Modified: Wed, 21 Dec 2022 12:20:58 GMT  
		Size: 334.8 KB (334765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bb1fb353f747aa2cdd4952aa366c48c03fd0a22dc2a88790e59ba8edd5c98d`  
		Last Modified: Wed, 21 Dec 2022 12:21:06 GMT  
		Size: 74.1 MB (74089601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:05aab2a99ce2a82114702ab96fad303931550f526d653ac46fc77160e779f287
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:a6d60e329c918cf340858effdd28e13d66a6bf0541b96e647242de597a386732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343186980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4431c3220c78f40fafe49622a3d2e51646341b4ac86ea5ad573e7c67e4c3e031`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 04:59:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04f6777c88ff80e0f77fdb7ff65116add73c3634a159f809353f1744c84a8d`  
		Last Modified: Fri, 09 Dec 2022 05:35:05 GMT  
		Size: 50.9 MB (50940037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7503ecddb0b97320554e87b25487d0bdfa37b7fe5c37bc47c4456fe68f03c`  
		Last Modified: Fri, 09 Dec 2022 05:34:57 GMT  
		Size: 340.3 KB (340328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805842103fd592ffb0abe0db2ae0b9e755b178666a0704448f5edfb2e374a42b`  
		Last Modified: Fri, 09 Dec 2022 05:35:09 GMT  
		Size: 79.6 MB (79603294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d17750dfa2dbd08fed5f26066b582ccf50451669e8978766e1cb48dd30391e6f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289283606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9be7b8f21dff9b49ad4024be643163437356117bb2dcebf68bea286629f273`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:14:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:16:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efeea9bf9b7ab77f23e367c89da5c0e5531f5addb65cf25bc0a5b5e83cf7f7b`  
		Last Modified: Fri, 09 Dec 2022 02:29:41 GMT  
		Size: 40.5 MB (40504997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e605d17caddb405dccfcc06092ec788bb817cd359400f2df0b99147c2b496`  
		Last Modified: Fri, 09 Dec 2022 02:29:35 GMT  
		Size: 340.3 KB (340279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19a17ff4caad94ebd5e6c31ff3d11a54ce63c9be19e1df0eb10e8f25280c743`  
		Last Modified: Fri, 09 Dec 2022 02:29:46 GMT  
		Size: 60.5 MB (60482408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f91972d4c1b3993884e1b4bb6202bc010a485b216aafdf67f0b02061198b2cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322850055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6efff5e9eebc1d010289b96f74b9b3c5b0e5331af7d6cfe3031d5ca016959d42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:46:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 02:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead157feea54418605c4179dd4abcec6c7d316435a84ff1165d0a9c5fb62c9f8`  
		Last Modified: Fri, 09 Dec 2022 03:23:41 GMT  
		Size: 45.2 MB (45203018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd364bf4779f23d7a2f96713796b5e10ebd7bddddf9dbd2af3537841a4e4c100`  
		Last Modified: Fri, 09 Dec 2022 03:23:36 GMT  
		Size: 340.3 KB (340337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c33ed43c56e3ea93d220e9ca8612a7f0bc0d26325ae93e7572f42a8175da45`  
		Last Modified: Fri, 09 Dec 2022 03:23:45 GMT  
		Size: 72.0 MB (71973023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:599a2ddce1c0eb6318a075538c3d4a61b53ba3be8c15a5ff87ddf2602b675439
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:41f06b60c2f4832e3b793bcf77e60ece183e367c71be52a71908c5323b562c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212303321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1729f0a46a3db62d35eb6f165e9db2c1206e9e0d19f6310b964a5c21de401b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:65b80df67588378ca238d3d62142164812673fdf322d992a8f07918492e4b2f5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187955922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ead31bf401dacb7152bb70492e97278c4a741dec405c01bb464090a2e0ff0bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c7cef327b88703f6ddf334ed0b91fbd57b4750c497e750e14d915d7968965d5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205333677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301f23e9604ae8f7bf722e91e092939973333c74ef5321fc2ddf415c7c55f429`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:ff12e51a96381a0c7c34fa5dbcbb911a0e441533f2e675b13fc500709a18bd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:89966fc74ab3551a125b04fea2b7fd1297c887e1b75c7300db89c9e5dd13468f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300553687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d777c39d82dfc632fbaf4792c635130dab511f386c4f9762ca82386a8ac32832`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:41 GMT
ADD file:c865da7afcf35b5a9538e63633f7e99ae4c40933cb8a0235e9704713042fba66 in / 
# Wed, 21 Dec 2022 01:20:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:00:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:00:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 11:00:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 11:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:01:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 11:01:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 11:01:37 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c7c50787e2da71205402343dd1233b3ca6ebe70c7e790f6ba7d856b81b893200`  
		Last Modified: Wed, 21 Dec 2022 01:24:55 GMT  
		Size: 50.4 MB (50448893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b052e3063dd5e1f5dd43ac9327c08a1f0ba5c05673755f0ddbc54eb8a47b68ed`  
		Last Modified: Wed, 21 Dec 2022 11:08:36 GMT  
		Size: 10.9 MB (10896939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83902353ad66fb52936b96293c207b00d5b37b587f35948ca0a2e679a1f0a0e`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cadf3ead30322d6c27a63204270292209d103c528b40928749587f9d7e136a`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c16a3a9b3a8fe00067d85297c8380ad068e3b1f484b284f35f9d54feaa04d`  
		Last Modified: Wed, 21 Dec 2022 11:09:08 GMT  
		Size: 239.2 MB (239205442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9168ac3a9e93b34a9b55bbd10385b07a62b2e6d6cc2c2ea2fde52bae7aeb96`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:10a4a8ca5f47bf3af732cfd6eedd0cc97e8dfb0478a5254bf23562b2bbbee66a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244527099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:854b760e1ee2468a1f009aac750b3f18b0d69c1e7f88efc93a0e51d8e0a4ea91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:12:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:12:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 12:12:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 12:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:13:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 12:13:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 12:13:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08619936cad6d315f51012474fa22f2fd8f1b475904aeeff8ab1ac9c94fb0770`  
		Last Modified: Wed, 21 Dec 2022 12:20:30 GMT  
		Size: 10.9 MB (10902542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49515cbca6d7dbd9df1f61795afce1f6540a7a7311f1e810e4e6119c9fe2b775`  
		Last Modified: Wed, 21 Dec 2022 12:20:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b1d3f149f7c168a510f4e797a86641439ab36f1672b64c32293d7f8c8501bc`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843956780ad36f94b7e0b598faa8c34f95b66ed491d15dc1b1d415e442f55810`  
		Last Modified: Wed, 21 Dec 2022 12:20:52 GMT  
		Size: 184.4 MB (184388328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689420f0e90e19012bdbc76769c6d25d3029bb1789f3f4e11b26ddfc71c98cb5`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:599a2ddce1c0eb6318a075538c3d4a61b53ba3be8c15a5ff87ddf2602b675439
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:41f06b60c2f4832e3b793bcf77e60ece183e367c71be52a71908c5323b562c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212303321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1729f0a46a3db62d35eb6f165e9db2c1206e9e0d19f6310b964a5c21de401b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:56:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:56:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:59:06 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:59:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:59:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529aee2e3a92be4f06b63d37bb43dc340b2268b625ca98a14645f4d8798dd5d`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccb893f642f161489ee8aa949f4f21b8ed3f1db954bad66ed7633d564944ea`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b53ddb82e9008abd52793465c9728a2624be314ea6a034a06de5d1d8f3ae0c`  
		Last Modified: Fri, 09 Dec 2022 05:34:48 GMT  
		Size: 177.0 MB (177017773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaad258b4a7ff918fe6fdb5378d5120d210256b218f6db6dd15037a06f7afb`  
		Last Modified: Fri, 09 Dec 2022 05:34:19 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:65b80df67588378ca238d3d62142164812673fdf322d992a8f07918492e4b2f5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187955922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ead31bf401dacb7152bb70492e97278c4a741dec405c01bb464090a2e0ff0bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:10:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:10:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:10:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:10:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:13:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:13:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:13:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0980f17f3871c61150f8cf58e565a617c7bd6c32e7f5b9c6b3b5db82ed585db3`  
		Last Modified: Fri, 09 Dec 2022 02:28:51 GMT  
		Size: 1.2 MB (1157105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba0da6f563b0477658b92d647844421ed559d9a8e27a5c22af6fc3331f2480`  
		Last Modified: Fri, 09 Dec 2022 02:28:49 GMT  
		Size: 4.7 MB (4680459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7279077448b46faa5746400fe5a6873f0f9c06e2c5ea412146151b28be9188ed`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad4197cb67bbb0e1bf14fd36da020e21265c002699e944c802762b6f162cdf`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6659920eeae5f2c8fcc9a50cea505670f64bb69c4e3bbfacfc3a93526be5c5`  
		Last Modified: Fri, 09 Dec 2022 02:29:22 GMT  
		Size: 157.5 MB (157526943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd88c1401d8f41679e81b08e3672e4bb5690194555ac55510eb7888d3922ac`  
		Last Modified: Fri, 09 Dec 2022 02:28:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c7cef327b88703f6ddf334ed0b91fbd57b4750c497e750e14d915d7968965d5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205333677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301f23e9604ae8f7bf722e91e092939973333c74ef5321fc2ddf415c7c55f429`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:43:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:43:52 GMT
ENV ROS_DISTRO=noetic
# Fri, 09 Dec 2022 02:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:46:20 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:46:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3639e209077f7e6226768f83798bd6aee04df07629d10667e99661522b3e9e1`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ee4c248f6cdad5e22c044f28a2d9159c24e1dcb39f9154871184edacf3cabd`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091bad4bf606b56e02a562e792d9baa2cad48286f053f702a84dec6af76aa12`  
		Last Modified: Fri, 09 Dec 2022 03:23:26 GMT  
		Size: 171.5 MB (171452281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34c3366b1680e763aa38bb22c6f742175c393c6accf12389013451361ffc5a`  
		Last Modified: Fri, 09 Dec 2022 03:22:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:598b008cacac6743996ece646095ea7bc541df9e59f596bf6e31d61721a17e71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:e8efe5ec7a288831e8eb1b5a9e2c173a9c312900bbbe59dc80844eee1abb18ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.3 MB (263319258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff57ad8fbd909490e0156720c4e9e97f452285302ae04bec39e0b796c0e72912`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:28:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:28:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05234a2ca3f99799e2c57496314b4624263eafbee96a0f893777beb97ea7ce`  
		Last Modified: Fri, 09 Dec 2022 05:42:38 GMT  
		Size: 84.9 MB (84913212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e6e140ca329314aaaf8dbf893f4da2b2a7fb9b39e07413401af0647ede7cd`  
		Last Modified: Fri, 09 Dec 2022 05:42:27 GMT  
		Size: 296.1 KB (296142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7518fc920f32812d31cd983d2b5acb69b60bda967f73fb5636ba865f169879d2`  
		Last Modified: Fri, 09 Dec 2022 05:42:26 GMT  
		Size: 2.4 KB (2439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0b0c0c22fc3780265c211bc70946a44bc02dfbd4fb75bb893049fe42b2bcf3`  
		Last Modified: Fri, 09 Dec 2022 05:42:30 GMT  
		Size: 23.2 MB (23214968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b9dc322cda9221089ecb2d5d0ce982bc57db8aca8161ba14bc203029909c45c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (255975788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27eece908402af996a06e21c4f7f063f1d2b73bb13c3a840327621edcb77ca0c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:17:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:17:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:18:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68d70c0c72d40b92fedcb34f5e67324f0587e422fb999228549b4570cf210c`  
		Last Modified: Fri, 09 Dec 2022 03:30:34 GMT  
		Size: 82.6 MB (82623980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71ea1b0029da51b11970243be13a8c989afa48826f3f2ed8e8a3d3c15c995b8`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 296.1 KB (296149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442e741c91b6ef65b80ac57fea831e491d848e222c0317f805bc1c44680e54f`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716c0c6c13f04dde21e2e28c2611e35c7fb2b0144f58f9560647aac6b87ebb12`  
		Last Modified: Fri, 09 Dec 2022 03:30:28 GMT  
		Size: 22.6 MB (22637964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:4dc057de9e1075632ddba4424246ef4921cea5052b385c15c66da7641122c032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:a24fd21c5027a73b0ca1d27c163ad7d5f6e37faea2a0a65c3f3917851b7eedb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1088316164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caa66eb605e44275849733a1a3e986bd1b0737e8629088a506bee1c439b8bd1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:28:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:28:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:31:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05234a2ca3f99799e2c57496314b4624263eafbee96a0f893777beb97ea7ce`  
		Last Modified: Fri, 09 Dec 2022 05:42:38 GMT  
		Size: 84.9 MB (84913212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e6e140ca329314aaaf8dbf893f4da2b2a7fb9b39e07413401af0647ede7cd`  
		Last Modified: Fri, 09 Dec 2022 05:42:27 GMT  
		Size: 296.1 KB (296142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7518fc920f32812d31cd983d2b5acb69b60bda967f73fb5636ba865f169879d2`  
		Last Modified: Fri, 09 Dec 2022 05:42:26 GMT  
		Size: 2.4 KB (2439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0b0c0c22fc3780265c211bc70946a44bc02dfbd4fb75bb893049fe42b2bcf3`  
		Last Modified: Fri, 09 Dec 2022 05:42:30 GMT  
		Size: 23.2 MB (23214968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4b9e5f0e6c2004cb5135d05f94dc4f4648ccccf27eb77a88f2706296983b05`  
		Last Modified: Fri, 09 Dec 2022 05:44:27 GMT  
		Size: 825.0 MB (824996906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fef5927e379964199e83e917a85176bc94b3cb9adb5277a64a81ca9f2656c926
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1038518525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320e65ea95fd2bd91317d473ccc97ec9a6c63210c7678a1209fea2e27468c6e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:17:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:17:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:18:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:19:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68d70c0c72d40b92fedcb34f5e67324f0587e422fb999228549b4570cf210c`  
		Last Modified: Fri, 09 Dec 2022 03:30:34 GMT  
		Size: 82.6 MB (82623980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71ea1b0029da51b11970243be13a8c989afa48826f3f2ed8e8a3d3c15c995b8`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 296.1 KB (296149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442e741c91b6ef65b80ac57fea831e491d848e222c0317f805bc1c44680e54f`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716c0c6c13f04dde21e2e28c2611e35c7fb2b0144f58f9560647aac6b87ebb12`  
		Last Modified: Fri, 09 Dec 2022 03:30:28 GMT  
		Size: 22.6 MB (22637964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51b998f8d6119899a34eade97d8511b9d337281b6d8f454813c6a4d5240f278`  
		Last Modified: Fri, 09 Dec 2022 03:32:06 GMT  
		Size: 782.5 MB (782542737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:4dc057de9e1075632ddba4424246ef4921cea5052b385c15c66da7641122c032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:a24fd21c5027a73b0ca1d27c163ad7d5f6e37faea2a0a65c3f3917851b7eedb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1088316164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caa66eb605e44275849733a1a3e986bd1b0737e8629088a506bee1c439b8bd1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:28:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:28:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:31:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05234a2ca3f99799e2c57496314b4624263eafbee96a0f893777beb97ea7ce`  
		Last Modified: Fri, 09 Dec 2022 05:42:38 GMT  
		Size: 84.9 MB (84913212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e6e140ca329314aaaf8dbf893f4da2b2a7fb9b39e07413401af0647ede7cd`  
		Last Modified: Fri, 09 Dec 2022 05:42:27 GMT  
		Size: 296.1 KB (296142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7518fc920f32812d31cd983d2b5acb69b60bda967f73fb5636ba865f169879d2`  
		Last Modified: Fri, 09 Dec 2022 05:42:26 GMT  
		Size: 2.4 KB (2439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0b0c0c22fc3780265c211bc70946a44bc02dfbd4fb75bb893049fe42b2bcf3`  
		Last Modified: Fri, 09 Dec 2022 05:42:30 GMT  
		Size: 23.2 MB (23214968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4b9e5f0e6c2004cb5135d05f94dc4f4648ccccf27eb77a88f2706296983b05`  
		Last Modified: Fri, 09 Dec 2022 05:44:27 GMT  
		Size: 825.0 MB (824996906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fef5927e379964199e83e917a85176bc94b3cb9adb5277a64a81ca9f2656c926
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1038518525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320e65ea95fd2bd91317d473ccc97ec9a6c63210c7678a1209fea2e27468c6e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:17:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:17:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:18:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:19:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68d70c0c72d40b92fedcb34f5e67324f0587e422fb999228549b4570cf210c`  
		Last Modified: Fri, 09 Dec 2022 03:30:34 GMT  
		Size: 82.6 MB (82623980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71ea1b0029da51b11970243be13a8c989afa48826f3f2ed8e8a3d3c15c995b8`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 296.1 KB (296149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442e741c91b6ef65b80ac57fea831e491d848e222c0317f805bc1c44680e54f`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716c0c6c13f04dde21e2e28c2611e35c7fb2b0144f58f9560647aac6b87ebb12`  
		Last Modified: Fri, 09 Dec 2022 03:30:28 GMT  
		Size: 22.6 MB (22637964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51b998f8d6119899a34eade97d8511b9d337281b6d8f454813c6a4d5240f278`  
		Last Modified: Fri, 09 Dec 2022 03:32:06 GMT  
		Size: 782.5 MB (782542737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:598b008cacac6743996ece646095ea7bc541df9e59f596bf6e31d61721a17e71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:e8efe5ec7a288831e8eb1b5a9e2c173a9c312900bbbe59dc80844eee1abb18ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.3 MB (263319258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff57ad8fbd909490e0156720c4e9e97f452285302ae04bec39e0b796c0e72912`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:28:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:28:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05234a2ca3f99799e2c57496314b4624263eafbee96a0f893777beb97ea7ce`  
		Last Modified: Fri, 09 Dec 2022 05:42:38 GMT  
		Size: 84.9 MB (84913212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e6e140ca329314aaaf8dbf893f4da2b2a7fb9b39e07413401af0647ede7cd`  
		Last Modified: Fri, 09 Dec 2022 05:42:27 GMT  
		Size: 296.1 KB (296142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7518fc920f32812d31cd983d2b5acb69b60bda967f73fb5636ba865f169879d2`  
		Last Modified: Fri, 09 Dec 2022 05:42:26 GMT  
		Size: 2.4 KB (2439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0b0c0c22fc3780265c211bc70946a44bc02dfbd4fb75bb893049fe42b2bcf3`  
		Last Modified: Fri, 09 Dec 2022 05:42:30 GMT  
		Size: 23.2 MB (23214968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b9dc322cda9221089ecb2d5d0ce982bc57db8aca8161ba14bc203029909c45c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (255975788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27eece908402af996a06e21c4f7f063f1d2b73bb13c3a840327621edcb77ca0c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:17:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:17:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:18:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68d70c0c72d40b92fedcb34f5e67324f0587e422fb999228549b4570cf210c`  
		Last Modified: Fri, 09 Dec 2022 03:30:34 GMT  
		Size: 82.6 MB (82623980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71ea1b0029da51b11970243be13a8c989afa48826f3f2ed8e8a3d3c15c995b8`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 296.1 KB (296149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442e741c91b6ef65b80ac57fea831e491d848e222c0317f805bc1c44680e54f`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716c0c6c13f04dde21e2e28c2611e35c7fb2b0144f58f9560647aac6b87ebb12`  
		Last Modified: Fri, 09 Dec 2022 03:30:28 GMT  
		Size: 22.6 MB (22637964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:598b008cacac6743996ece646095ea7bc541df9e59f596bf6e31d61721a17e71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e8efe5ec7a288831e8eb1b5a9e2c173a9c312900bbbe59dc80844eee1abb18ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.3 MB (263319258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff57ad8fbd909490e0156720c4e9e97f452285302ae04bec39e0b796c0e72912`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:28:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 05:28:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 05:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05234a2ca3f99799e2c57496314b4624263eafbee96a0f893777beb97ea7ce`  
		Last Modified: Fri, 09 Dec 2022 05:42:38 GMT  
		Size: 84.9 MB (84913212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e6e140ca329314aaaf8dbf893f4da2b2a7fb9b39e07413401af0647ede7cd`  
		Last Modified: Fri, 09 Dec 2022 05:42:27 GMT  
		Size: 296.1 KB (296142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7518fc920f32812d31cd983d2b5acb69b60bda967f73fb5636ba865f169879d2`  
		Last Modified: Fri, 09 Dec 2022 05:42:26 GMT  
		Size: 2.4 KB (2439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0b0c0c22fc3780265c211bc70946a44bc02dfbd4fb75bb893049fe42b2bcf3`  
		Last Modified: Fri, 09 Dec 2022 05:42:30 GMT  
		Size: 23.2 MB (23214968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b9dc322cda9221089ecb2d5d0ce982bc57db8aca8161ba14bc203029909c45c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (255975788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27eece908402af996a06e21c4f7f063f1d2b73bb13c3a840327621edcb77ca0c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:17:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 09 Dec 2022 03:17:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 09 Dec 2022 03:18:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68d70c0c72d40b92fedcb34f5e67324f0587e422fb999228549b4570cf210c`  
		Last Modified: Fri, 09 Dec 2022 03:30:34 GMT  
		Size: 82.6 MB (82623980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71ea1b0029da51b11970243be13a8c989afa48826f3f2ed8e8a3d3c15c995b8`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 296.1 KB (296149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442e741c91b6ef65b80ac57fea831e491d848e222c0317f805bc1c44680e54f`  
		Last Modified: Fri, 09 Dec 2022 03:30:25 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716c0c6c13f04dde21e2e28c2611e35c7fb2b0144f58f9560647aac6b87ebb12`  
		Last Modified: Fri, 09 Dec 2022 03:30:28 GMT  
		Size: 22.6 MB (22637964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:dac2e84421d0fd0d48d107cadec0db3d8504a762e5a2a455b0b798eec9c0562a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:065c6be832bf0f49c7b8b475722ca3b6c0f9cbd8f2142a0f5089b56c98aedc08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154892497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c02bb72a5aef4c2d62f39624f29108632e9837e9332fdeece0ad4aa4bb880e56`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:652e31d47b489d44081f76e2409317b82cf33ad3d68e715f631364a42cbd652c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150415273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d2eec9d0c6bc0257b7929016428ad9fb51fc2b8069dcbc790e784604ec876c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:dac2e84421d0fd0d48d107cadec0db3d8504a762e5a2a455b0b798eec9c0562a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:065c6be832bf0f49c7b8b475722ca3b6c0f9cbd8f2142a0f5089b56c98aedc08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154892497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c02bb72a5aef4c2d62f39624f29108632e9837e9332fdeece0ad4aa4bb880e56`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 05:14:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:15:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 05:15:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 05:15:02 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 05:15:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 05:27:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 05:28:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 05:28:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 05:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 05:28:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a075a4212270474a7d05b2a3df4d10124cfe8bea3a09061f3743bdfdeea620`  
		Last Modified: Fri, 09 Dec 2022 05:39:22 GMT  
		Size: 1.2 MB (1168785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca9afe1ea65f3443c92169383384dedafa95933b2e054106c0de21b6c34d48`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 3.8 MB (3828147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd221bf00513721700dbf17f757c3d2c694e4f5866cc10d522aca08d918542`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6bb9c524a1795566113eec993f29c6509ea63f84d84b6172832d962dad457`  
		Last Modified: Fri, 09 Dec 2022 05:39:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213055ab1d8b2c0a651cebe6546d993f2dc65a5926293b42c8359f4215af9a9a`  
		Last Modified: Fri, 09 Dec 2022 05:42:18 GMT  
		Size: 119.5 MB (119464440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79d994318b8f2df45429b9a7ba487600e2dfd1cef4d8d6efce7847bcd4ca2aa`  
		Last Modified: Fri, 09 Dec 2022 05:41:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:652e31d47b489d44081f76e2409317b82cf33ad3d68e715f631364a42cbd652c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150415273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d2eec9d0c6bc0257b7929016428ad9fb51fc2b8069dcbc790e784604ec876c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:01:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:02:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 09 Dec 2022 03:02:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 03:02:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 03:16:50 GMT
ENV ROS_DISTRO=rolling
# Fri, 09 Dec 2022 03:17:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:17:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 09 Dec 2022 03:17:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 03:17:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8dc3e3065c6ea4d11a008128adae56cbb9f13628e58b8aaf334329f716e92`  
		Last Modified: Fri, 09 Dec 2022 03:27:38 GMT  
		Size: 1.2 MB (1170314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8bd153ff56b0dca3f778fd85306914b8e9f50c343a01fbbdc20f9e53b1ea`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 3.8 MB (3801750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b23c139b344480421c4eacff1b9cfae6f881dbab5c213d1a062e9aa523eeb1`  
		Last Modified: Fri, 09 Dec 2022 03:27:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39b13b1db0fb60b86f2083c60b57ddb444d12dd03f8ed55a5a91f2bbe109a5c`  
		Last Modified: Fri, 09 Dec 2022 03:27:36 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96411d012665da3319068ba881d140456336fbcc47a6a1aa53f48c3c12c29e0`  
		Last Modified: Fri, 09 Dec 2022 03:30:16 GMT  
		Size: 117.1 MB (117056322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4f105c7753b16afb5f4e2d028098cfe6bc71161732ffc08401de22735af986`  
		Last Modified: Fri, 09 Dec 2022 03:29:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
