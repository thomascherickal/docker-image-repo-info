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
-	[`ros:kinetic`](#roskinetic)
-	[`ros:kinetic-perception`](#roskinetic-perception)
-	[`ros:kinetic-perception-xenial`](#roskinetic-perception-xenial)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-robot-xenial`](#roskinetic-robot-xenial)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic-ros-base-xenial`](#roskinetic-ros-base-xenial)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-core-xenial`](#roskinetic-ros-core-xenial)
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
$ docker pull ros@sha256:f6cddb1159e664afc1d8b3c556f0dd8fece7ab03a94887cab5e2f977ebb4e397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:b84dc55dec6da1ab52de0b8b11377caa867e9c7d37be12ae66752c2e203f8f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232376681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5459f09fa2f11b0c8d454c2b00df1a21b52549f1af3276dfe4230bb864e03caf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8939446e904c58630b7211dec304744f9f5b26cc0eac113bff1b31f26d85bb46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208507337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107fb98757cb59013e35f1ae50e6cc673dd9da695e44bdb46a0eda65916174ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:22:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:22:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0451cef7bd337ebad4e48e1f3eb634e9417d75ed87155dec3fff664d0fb391`  
		Last Modified: Fri, 18 Jun 2021 01:40:37 GMT  
		Size: 61.0 MB (60970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbc1eed614e6ee80416147df177c36ea5f19940e8b72dc57563513f40822e46`  
		Last Modified: Fri, 18 Jun 2021 01:40:27 GMT  
		Size: 235.2 KB (235206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620e4cae49af2590062e84bff0deb34e1e15c08c2a7a5e37384c230b4b191da`  
		Last Modified: Fri, 18 Jun 2021 01:40:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00222544fae9505236ccdf441360698a6d77df31c78ad609d422651622b07d`  
		Last Modified: Fri, 18 Jun 2021 01:40:29 GMT  
		Size: 9.3 MB (9298549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:f6cddb1159e664afc1d8b3c556f0dd8fece7ab03a94887cab5e2f977ebb4e397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b84dc55dec6da1ab52de0b8b11377caa867e9c7d37be12ae66752c2e203f8f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232376681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5459f09fa2f11b0c8d454c2b00df1a21b52549f1af3276dfe4230bb864e03caf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8939446e904c58630b7211dec304744f9f5b26cc0eac113bff1b31f26d85bb46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208507337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107fb98757cb59013e35f1ae50e6cc673dd9da695e44bdb46a0eda65916174ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:22:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:22:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0451cef7bd337ebad4e48e1f3eb634e9417d75ed87155dec3fff664d0fb391`  
		Last Modified: Fri, 18 Jun 2021 01:40:37 GMT  
		Size: 61.0 MB (60970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbc1eed614e6ee80416147df177c36ea5f19940e8b72dc57563513f40822e46`  
		Last Modified: Fri, 18 Jun 2021 01:40:27 GMT  
		Size: 235.2 KB (235206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620e4cae49af2590062e84bff0deb34e1e15c08c2a7a5e37384c230b4b191da`  
		Last Modified: Fri, 18 Jun 2021 01:40:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00222544fae9505236ccdf441360698a6d77df31c78ad609d422651622b07d`  
		Last Modified: Fri, 18 Jun 2021 01:40:29 GMT  
		Size: 9.3 MB (9298549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:f6cddb1159e664afc1d8b3c556f0dd8fece7ab03a94887cab5e2f977ebb4e397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:b84dc55dec6da1ab52de0b8b11377caa867e9c7d37be12ae66752c2e203f8f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232376681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5459f09fa2f11b0c8d454c2b00df1a21b52549f1af3276dfe4230bb864e03caf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8939446e904c58630b7211dec304744f9f5b26cc0eac113bff1b31f26d85bb46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208507337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107fb98757cb59013e35f1ae50e6cc673dd9da695e44bdb46a0eda65916174ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:22:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:22:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0451cef7bd337ebad4e48e1f3eb634e9417d75ed87155dec3fff664d0fb391`  
		Last Modified: Fri, 18 Jun 2021 01:40:37 GMT  
		Size: 61.0 MB (60970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbc1eed614e6ee80416147df177c36ea5f19940e8b72dc57563513f40822e46`  
		Last Modified: Fri, 18 Jun 2021 01:40:27 GMT  
		Size: 235.2 KB (235206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620e4cae49af2590062e84bff0deb34e1e15c08c2a7a5e37384c230b4b191da`  
		Last Modified: Fri, 18 Jun 2021 01:40:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00222544fae9505236ccdf441360698a6d77df31c78ad609d422651622b07d`  
		Last Modified: Fri, 18 Jun 2021 01:40:29 GMT  
		Size: 9.3 MB (9298549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:91ebb2f3165b3dcb404bdb74efb111b8f6324d561d4b64a1f02dcbb2c0974cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:08ed3e793d1d05d81c20e555086116714ad00e7b9b83dec4469c5fbc92334dc7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155253875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1800f5f7b8de233f9c8d356d706edb389a9aba5d623be5ab84fd22e1a313632`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c564f497be5099ad4d60ef5bea9efae21f3edacf39527100c6d10ff5a4c08a9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138001462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b148ac018b04d103f2229b85eb8ec22dfc71c071d3832586490e6469d4f91e1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:91ebb2f3165b3dcb404bdb74efb111b8f6324d561d4b64a1f02dcbb2c0974cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:08ed3e793d1d05d81c20e555086116714ad00e7b9b83dec4469c5fbc92334dc7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155253875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1800f5f7b8de233f9c8d356d706edb389a9aba5d623be5ab84fd22e1a313632`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c564f497be5099ad4d60ef5bea9efae21f3edacf39527100c6d10ff5a4c08a9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138001462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b148ac018b04d103f2229b85eb8ec22dfc71c071d3832586490e6469d4f91e1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:e688eda514b441d6caa62d9b8574b96ac935abe696b3c46de022f9cdde2788ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:dfbb3efe894b0d339be4791b3618ac6046916411ab7b585fd5581e107bc4c799
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.2 MB (341235143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2552de4ac28f449e936791a67cbacf4e8cad07b12691c8edfd75918112425b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:14:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:14:53 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:14:54 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Jun 2021 02:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:15:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:15:37 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2964df2e550f0cd1ffb296650e598f8a3f82a335be6e2d7c65a5604a52f0ff4`  
		Last Modified: Fri, 18 Jun 2021 02:31:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaa0674c4d488fb04a402fc29cb300083d69b5b05186a931a8f2b14bc6b13f8`  
		Last Modified: Fri, 18 Jun 2021 02:31:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151152fa8fce96085f35456e3200517edf4347b179666f5e5ac41efe41c82ae`  
		Last Modified: Fri, 18 Jun 2021 02:31:49 GMT  
		Size: 76.1 MB (76122813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c606caea6666d241c2dc2f07c1a9ce07289911380c03552df011518e5795e0e`  
		Last Modified: Fri, 18 Jun 2021 02:31:36 GMT  
		Size: 32.7 MB (32735024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce4b64fcef5d56f7631c30d70ffb79d60c380bd2215260b656c73eaebac9edf`  
		Last Modified: Fri, 18 Jun 2021 02:31:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c6debd55f4631bad6f7ac8fe11a907dd6967ceea1f568f7850c08e6ac9f456a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309772847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107c6d8fac51aca5505a389265f9265ef4325abc5ac356613e91f952acdc04b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:22:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:22:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:23:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:23:05 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 01:23:05 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Jun 2021 01:23:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:47 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0451cef7bd337ebad4e48e1f3eb634e9417d75ed87155dec3fff664d0fb391`  
		Last Modified: Fri, 18 Jun 2021 01:40:37 GMT  
		Size: 61.0 MB (60970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbc1eed614e6ee80416147df177c36ea5f19940e8b72dc57563513f40822e46`  
		Last Modified: Fri, 18 Jun 2021 01:40:27 GMT  
		Size: 235.2 KB (235206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620e4cae49af2590062e84bff0deb34e1e15c08c2a7a5e37384c230b4b191da`  
		Last Modified: Fri, 18 Jun 2021 01:40:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00222544fae9505236ccdf441360698a6d77df31c78ad609d422651622b07d`  
		Last Modified: Fri, 18 Jun 2021 01:40:29 GMT  
		Size: 9.3 MB (9298549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6126d7df33636826e555fbaebc53de7750b9f565cb3e355313ac25991bafd9`  
		Last Modified: Fri, 18 Jun 2021 01:40:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564212a83d4620c999f2ed43ef5d8f706ff435d6c372003c92054952f7066ba6`  
		Last Modified: Fri, 18 Jun 2021 01:40:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb80d127dc33d452e64dbf065ad9c54e1d9ca400c07025fbfc45d56b4617d383`  
		Last Modified: Fri, 18 Jun 2021 01:41:19 GMT  
		Size: 76.2 MB (76155609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe8281eafd1aac4e37e054cb97ede05e655c6044ff944f62c08a7fa8dbdcc6`  
		Last Modified: Fri, 18 Jun 2021 01:41:03 GMT  
		Size: 25.1 MB (25109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ea0918067dc91e89147b0f2e100549ea60f6eecedbac62534487cacfe150b6`  
		Last Modified: Fri, 18 Jun 2021 01:40:58 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:e688eda514b441d6caa62d9b8574b96ac935abe696b3c46de022f9cdde2788ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:dfbb3efe894b0d339be4791b3618ac6046916411ab7b585fd5581e107bc4c799
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.2 MB (341235143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2552de4ac28f449e936791a67cbacf4e8cad07b12691c8edfd75918112425b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:14:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:14:53 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:14:54 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Jun 2021 02:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:15:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:15:37 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2964df2e550f0cd1ffb296650e598f8a3f82a335be6e2d7c65a5604a52f0ff4`  
		Last Modified: Fri, 18 Jun 2021 02:31:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaa0674c4d488fb04a402fc29cb300083d69b5b05186a931a8f2b14bc6b13f8`  
		Last Modified: Fri, 18 Jun 2021 02:31:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151152fa8fce96085f35456e3200517edf4347b179666f5e5ac41efe41c82ae`  
		Last Modified: Fri, 18 Jun 2021 02:31:49 GMT  
		Size: 76.1 MB (76122813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c606caea6666d241c2dc2f07c1a9ce07289911380c03552df011518e5795e0e`  
		Last Modified: Fri, 18 Jun 2021 02:31:36 GMT  
		Size: 32.7 MB (32735024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce4b64fcef5d56f7631c30d70ffb79d60c380bd2215260b656c73eaebac9edf`  
		Last Modified: Fri, 18 Jun 2021 02:31:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c6debd55f4631bad6f7ac8fe11a907dd6967ceea1f568f7850c08e6ac9f456a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309772847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107c6d8fac51aca5505a389265f9265ef4325abc5ac356613e91f952acdc04b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:22:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:22:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:23:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:23:05 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 01:23:05 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Jun 2021 01:23:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:47 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0451cef7bd337ebad4e48e1f3eb634e9417d75ed87155dec3fff664d0fb391`  
		Last Modified: Fri, 18 Jun 2021 01:40:37 GMT  
		Size: 61.0 MB (60970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbc1eed614e6ee80416147df177c36ea5f19940e8b72dc57563513f40822e46`  
		Last Modified: Fri, 18 Jun 2021 01:40:27 GMT  
		Size: 235.2 KB (235206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620e4cae49af2590062e84bff0deb34e1e15c08c2a7a5e37384c230b4b191da`  
		Last Modified: Fri, 18 Jun 2021 01:40:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00222544fae9505236ccdf441360698a6d77df31c78ad609d422651622b07d`  
		Last Modified: Fri, 18 Jun 2021 01:40:29 GMT  
		Size: 9.3 MB (9298549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6126d7df33636826e555fbaebc53de7750b9f565cb3e355313ac25991bafd9`  
		Last Modified: Fri, 18 Jun 2021 01:40:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564212a83d4620c999f2ed43ef5d8f706ff435d6c372003c92054952f7066ba6`  
		Last Modified: Fri, 18 Jun 2021 01:40:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb80d127dc33d452e64dbf065ad9c54e1d9ca400c07025fbfc45d56b4617d383`  
		Last Modified: Fri, 18 Jun 2021 01:41:19 GMT  
		Size: 76.2 MB (76155609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe8281eafd1aac4e37e054cb97ede05e655c6044ff944f62c08a7fa8dbdcc6`  
		Last Modified: Fri, 18 Jun 2021 01:41:03 GMT  
		Size: 25.1 MB (25109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ea0918067dc91e89147b0f2e100549ea60f6eecedbac62534487cacfe150b6`  
		Last Modified: Fri, 18 Jun 2021 01:40:58 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:45889ee536e67eaf0377b89cbc8c8050be4a44b3ab0f1651f194fe8ca2d95923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:99ad4ad48afa1e48a734d73cce2f9e218ddde5a49ee792589774556964f3a99b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227781075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:717c275e46091543e1e819d2bc302f4a3145db9a83fe953f0dbc53d51efcb182`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:16:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:16:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9f55b4fa18ae28d3d3490dbf2e89ec6b258acaced76fab09c769e7c21738f2`  
		Last Modified: Fri, 18 Jun 2021 02:32:48 GMT  
		Size: 66.6 MB (66550544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9274976ef70285b0e42376a86ed012534d5a01283c03c9fdda991545c3c11`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 234.4 KB (234425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10677ba132e2f8550410ea57e748edc342b44c8445b594c14a698f113c9ffe8a`  
		Last Modified: Fri, 18 Jun 2021 02:32:35 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d6631a8510e42592ff9485f745b27133e502c2ba2c621ec936e3ac56caab4`  
		Last Modified: Fri, 18 Jun 2021 02:32:41 GMT  
		Size: 22.1 MB (22095295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:677b3bb841d1ae79f14b1bac4ce11f108f5392e05d9c7fe109b78c3e71f82b44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216445420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910f544a3cc887501e4da6d0f012f779fbbac7c456988c5f2c389ebac68b6eaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:25:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:25:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63335e56c7209ab61e062d6938b7c35ea66a035c16c0da9eead06aec55a6e421`  
		Last Modified: Fri, 18 Jun 2021 01:42:19 GMT  
		Size: 60.9 MB (60920663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c81783b2c87d108d80f56dd45dfee5ef77561810c5d09f5b4cb8798fbe1677`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 234.4 KB (234418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa178075a0611f211a97568d17fbb8ae885c3ceb93a304e288934b729af49a`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aca8c035cfe4288740839b4acc527bcc1ccf3923cd663119acfb3b35bb2e4d`  
		Last Modified: Fri, 18 Jun 2021 01:42:12 GMT  
		Size: 21.4 MB (21430620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:45889ee536e67eaf0377b89cbc8c8050be4a44b3ab0f1651f194fe8ca2d95923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:99ad4ad48afa1e48a734d73cce2f9e218ddde5a49ee792589774556964f3a99b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227781075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:717c275e46091543e1e819d2bc302f4a3145db9a83fe953f0dbc53d51efcb182`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:16:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:16:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9f55b4fa18ae28d3d3490dbf2e89ec6b258acaced76fab09c769e7c21738f2`  
		Last Modified: Fri, 18 Jun 2021 02:32:48 GMT  
		Size: 66.6 MB (66550544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9274976ef70285b0e42376a86ed012534d5a01283c03c9fdda991545c3c11`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 234.4 KB (234425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10677ba132e2f8550410ea57e748edc342b44c8445b594c14a698f113c9ffe8a`  
		Last Modified: Fri, 18 Jun 2021 02:32:35 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d6631a8510e42592ff9485f745b27133e502c2ba2c621ec936e3ac56caab4`  
		Last Modified: Fri, 18 Jun 2021 02:32:41 GMT  
		Size: 22.1 MB (22095295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:677b3bb841d1ae79f14b1bac4ce11f108f5392e05d9c7fe109b78c3e71f82b44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216445420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910f544a3cc887501e4da6d0f012f779fbbac7c456988c5f2c389ebac68b6eaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:25:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:25:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63335e56c7209ab61e062d6938b7c35ea66a035c16c0da9eead06aec55a6e421`  
		Last Modified: Fri, 18 Jun 2021 01:42:19 GMT  
		Size: 60.9 MB (60920663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c81783b2c87d108d80f56dd45dfee5ef77561810c5d09f5b4cb8798fbe1677`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 234.4 KB (234418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa178075a0611f211a97568d17fbb8ae885c3ceb93a304e288934b729af49a`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aca8c035cfe4288740839b4acc527bcc1ccf3923cd663119acfb3b35bb2e4d`  
		Last Modified: Fri, 18 Jun 2021 01:42:12 GMT  
		Size: 21.4 MB (21430620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:45889ee536e67eaf0377b89cbc8c8050be4a44b3ab0f1651f194fe8ca2d95923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:99ad4ad48afa1e48a734d73cce2f9e218ddde5a49ee792589774556964f3a99b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227781075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:717c275e46091543e1e819d2bc302f4a3145db9a83fe953f0dbc53d51efcb182`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:16:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:16:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9f55b4fa18ae28d3d3490dbf2e89ec6b258acaced76fab09c769e7c21738f2`  
		Last Modified: Fri, 18 Jun 2021 02:32:48 GMT  
		Size: 66.6 MB (66550544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9274976ef70285b0e42376a86ed012534d5a01283c03c9fdda991545c3c11`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 234.4 KB (234425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10677ba132e2f8550410ea57e748edc342b44c8445b594c14a698f113c9ffe8a`  
		Last Modified: Fri, 18 Jun 2021 02:32:35 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d6631a8510e42592ff9485f745b27133e502c2ba2c621ec936e3ac56caab4`  
		Last Modified: Fri, 18 Jun 2021 02:32:41 GMT  
		Size: 22.1 MB (22095295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:677b3bb841d1ae79f14b1bac4ce11f108f5392e05d9c7fe109b78c3e71f82b44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216445420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910f544a3cc887501e4da6d0f012f779fbbac7c456988c5f2c389ebac68b6eaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:25:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:25:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63335e56c7209ab61e062d6938b7c35ea66a035c16c0da9eead06aec55a6e421`  
		Last Modified: Fri, 18 Jun 2021 01:42:19 GMT  
		Size: 60.9 MB (60920663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c81783b2c87d108d80f56dd45dfee5ef77561810c5d09f5b4cb8798fbe1677`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 234.4 KB (234418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa178075a0611f211a97568d17fbb8ae885c3ceb93a304e288934b729af49a`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aca8c035cfe4288740839b4acc527bcc1ccf3923cd663119acfb3b35bb2e4d`  
		Last Modified: Fri, 18 Jun 2021 01:42:12 GMT  
		Size: 21.4 MB (21430620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:41835752ff6496be2aa4921d1dbd36b624f43fb78b21fbb6c2f8b81861e1c540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:bc6c52fb0931ae4b1c0d3e73194c04582d71a13bc5215f487aad99efb071d8d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138898810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ce07622c2be357d5cc1ad486888a7cdc337d1cbfed8bf4e7d0c1c1042eeff9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9095030e395ee371749102e61169c8509ddb729495f54dd80f4cd5b2cdc60b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133857683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b2d0b9223a701f3f2373e21502550e43266e5ac0e89dfccce316ba0576820e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:41835752ff6496be2aa4921d1dbd36b624f43fb78b21fbb6c2f8b81861e1c540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:bc6c52fb0931ae4b1c0d3e73194c04582d71a13bc5215f487aad99efb071d8d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138898810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ce07622c2be357d5cc1ad486888a7cdc337d1cbfed8bf4e7d0c1c1042eeff9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9095030e395ee371749102e61169c8509ddb729495f54dd80f4cd5b2cdc60b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133857683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b2d0b9223a701f3f2373e21502550e43266e5ac0e89dfccce316ba0576820e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:b3016ad8fa5ce0f1964beedf891d88ba20c038f59a570b6eccb39fd5135e12f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:81a25ad83d26c179eb9b63b60933fc77f20c8cc68dfae1b168b542510709ffb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322553266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:343d6ece9ede76a8dbc169b285948d227c28b301b0ab37f47764f57ece3ec6b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:16:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:16:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:17:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:17:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:17:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:17:25 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Jun 2021 02:17:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:00 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9f55b4fa18ae28d3d3490dbf2e89ec6b258acaced76fab09c769e7c21738f2`  
		Last Modified: Fri, 18 Jun 2021 02:32:48 GMT  
		Size: 66.6 MB (66550544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9274976ef70285b0e42376a86ed012534d5a01283c03c9fdda991545c3c11`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 234.4 KB (234425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10677ba132e2f8550410ea57e748edc342b44c8445b594c14a698f113c9ffe8a`  
		Last Modified: Fri, 18 Jun 2021 02:32:35 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d6631a8510e42592ff9485f745b27133e502c2ba2c621ec936e3ac56caab4`  
		Last Modified: Fri, 18 Jun 2021 02:32:41 GMT  
		Size: 22.1 MB (22095295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67b827799f8410ffac85eacd7ba4da0d2375ae6a99c5c45f8c2f7688f014371`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe4710e4bf4c1167669a16f859d5cdb27c0eecfe90e01110558b697210a403`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada466ddc6b96b7af9abc72a23c6e7cc55a74162f8fa73ce97996ac018ea43a4`  
		Last Modified: Fri, 18 Jun 2021 02:33:24 GMT  
		Size: 78.4 MB (78409357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6db6cddc1ed7a70ccdeb1610359ec4b968e5536cfe49642b1f063dd9d4d6f9`  
		Last Modified: Fri, 18 Jun 2021 02:33:07 GMT  
		Size: 16.4 MB (16362214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf26bba415264851b5c953e79eccd6bdf209638624ab654fc27475f021aeef7`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3ce6570b41159f145ede08290de39f0094e22f0ef182413751d1dbc79a175b9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.7 MB (310704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8779df7ca086e881603699755bb16d974ea331ed1bfc2ad5a90ae1de78a09016`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:25:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:25:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:25:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:25:41 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 01:25:41 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Jun 2021 01:26:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:16 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63335e56c7209ab61e062d6938b7c35ea66a035c16c0da9eead06aec55a6e421`  
		Last Modified: Fri, 18 Jun 2021 01:42:19 GMT  
		Size: 60.9 MB (60920663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c81783b2c87d108d80f56dd45dfee5ef77561810c5d09f5b4cb8798fbe1677`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 234.4 KB (234418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa178075a0611f211a97568d17fbb8ae885c3ceb93a304e288934b729af49a`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aca8c035cfe4288740839b4acc527bcc1ccf3923cd663119acfb3b35bb2e4d`  
		Last Modified: Fri, 18 Jun 2021 01:42:12 GMT  
		Size: 21.4 MB (21430620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8827e22752ca2a0e9f9a2339c50fee3ea8f706a7c9c0c7090522d075b58f91`  
		Last Modified: Fri, 18 Jun 2021 01:42:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776f2b10add4db42bb4452a5002747bc6fc661c470de95c4ce386321e198a80c`  
		Last Modified: Fri, 18 Jun 2021 01:42:36 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823da43639f3474623e51135f7b66cafabc795dac90d3795475b6d7971a87df5`  
		Last Modified: Fri, 18 Jun 2021 01:42:58 GMT  
		Size: 78.4 MB (78368758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50b48efe0b3fbc4d4be12bfd497acb25e0e398faf3b7f95785e431421c6d61`  
		Last Modified: Fri, 18 Jun 2021 01:42:40 GMT  
		Size: 15.9 MB (15889849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8d1eca4f5cbdc522d300100dc2ca11fd25c67328a3bab9a11f07c2dea52774`  
		Last Modified: Fri, 18 Jun 2021 01:42:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:b3016ad8fa5ce0f1964beedf891d88ba20c038f59a570b6eccb39fd5135e12f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:81a25ad83d26c179eb9b63b60933fc77f20c8cc68dfae1b168b542510709ffb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322553266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:343d6ece9ede76a8dbc169b285948d227c28b301b0ab37f47764f57ece3ec6b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:16:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:16:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:17:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:17:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:17:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:17:25 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Jun 2021 02:17:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:00 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9f55b4fa18ae28d3d3490dbf2e89ec6b258acaced76fab09c769e7c21738f2`  
		Last Modified: Fri, 18 Jun 2021 02:32:48 GMT  
		Size: 66.6 MB (66550544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9274976ef70285b0e42376a86ed012534d5a01283c03c9fdda991545c3c11`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 234.4 KB (234425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10677ba132e2f8550410ea57e748edc342b44c8445b594c14a698f113c9ffe8a`  
		Last Modified: Fri, 18 Jun 2021 02:32:35 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d6631a8510e42592ff9485f745b27133e502c2ba2c621ec936e3ac56caab4`  
		Last Modified: Fri, 18 Jun 2021 02:32:41 GMT  
		Size: 22.1 MB (22095295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67b827799f8410ffac85eacd7ba4da0d2375ae6a99c5c45f8c2f7688f014371`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe4710e4bf4c1167669a16f859d5cdb27c0eecfe90e01110558b697210a403`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada466ddc6b96b7af9abc72a23c6e7cc55a74162f8fa73ce97996ac018ea43a4`  
		Last Modified: Fri, 18 Jun 2021 02:33:24 GMT  
		Size: 78.4 MB (78409357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6db6cddc1ed7a70ccdeb1610359ec4b968e5536cfe49642b1f063dd9d4d6f9`  
		Last Modified: Fri, 18 Jun 2021 02:33:07 GMT  
		Size: 16.4 MB (16362214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf26bba415264851b5c953e79eccd6bdf209638624ab654fc27475f021aeef7`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3ce6570b41159f145ede08290de39f0094e22f0ef182413751d1dbc79a175b9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.7 MB (310704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8779df7ca086e881603699755bb16d974ea331ed1bfc2ad5a90ae1de78a09016`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:23:55 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 01:24:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:24:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:24:36 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:25:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:25:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:25:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:25:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:25:41 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 01:25:41 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Jun 2021 01:26:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:16 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c281cd5faa4737a808df230ea8794460973abcfe6c9b9b340613dd43e4474`  
		Last Modified: Fri, 18 Jun 2021 01:41:56 GMT  
		Size: 100.0 MB (99999949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bbebd3cebc33ba53aa35ed6230d6a5f209def2bfc680adf558778cbcc8405`  
		Last Modified: Fri, 18 Jun 2021 01:41:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63335e56c7209ab61e062d6938b7c35ea66a035c16c0da9eead06aec55a6e421`  
		Last Modified: Fri, 18 Jun 2021 01:42:19 GMT  
		Size: 60.9 MB (60920663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c81783b2c87d108d80f56dd45dfee5ef77561810c5d09f5b4cb8798fbe1677`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 234.4 KB (234418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa178075a0611f211a97568d17fbb8ae885c3ceb93a304e288934b729af49a`  
		Last Modified: Fri, 18 Jun 2021 01:42:08 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aca8c035cfe4288740839b4acc527bcc1ccf3923cd663119acfb3b35bb2e4d`  
		Last Modified: Fri, 18 Jun 2021 01:42:12 GMT  
		Size: 21.4 MB (21430620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8827e22752ca2a0e9f9a2339c50fee3ea8f706a7c9c0c7090522d075b58f91`  
		Last Modified: Fri, 18 Jun 2021 01:42:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776f2b10add4db42bb4452a5002747bc6fc661c470de95c4ce386321e198a80c`  
		Last Modified: Fri, 18 Jun 2021 01:42:36 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823da43639f3474623e51135f7b66cafabc795dac90d3795475b6d7971a87df5`  
		Last Modified: Fri, 18 Jun 2021 01:42:58 GMT  
		Size: 78.4 MB (78368758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50b48efe0b3fbc4d4be12bfd497acb25e0e398faf3b7f95785e431421c6d61`  
		Last Modified: Fri, 18 Jun 2021 01:42:40 GMT  
		Size: 15.9 MB (15889849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8d1eca4f5cbdc522d300100dc2ca11fd25c67328a3bab9a11f07c2dea52774`  
		Last Modified: Fri, 18 Jun 2021 01:42:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic`

```console
$ docker pull ros@sha256:29c7cb9305475baba4aee5c0b944dca3514c38c9d7b90c5830dfc72ca454ceab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:04f8a0de3d163dbaa208590c46ed4a41445fc78e0074731c29d47b81d28a8506
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.2 MB (360168372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c5711abb297816bcc85d771acaacd9766a66bf679ef9d342e9ef815f158e96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:6aa9871749c213a24f429a77db3f062a7de532602524cd47caf3751794ffb053
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311677739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c7a5e78352deae3cc66bc4c705b3708ce93a311358b919ed921274c9a6ed5ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d412ad704c05401d9fc89b01cfa35678a6b552787b11fa9431a9c2a7619848fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325644424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3dd6b7a1f0ae9bd26af7a0e76f80e51e58ce4756d3e7a8f2dd853f3ea01e28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:a7f16cf9a61d059c2f655546e7c09a973b5e4d97e54091223599a94535f91ca9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:72a0d008f4bea8fb2c0e0e334f54631a620e16b8c775bd17e1c4b9b7444f2482
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.8 MB (676818460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6a45d8a3e903b25bb7347511fc59162735b9dea255289f8f5d562a293900566`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adac9976a40b77f3bb66a8df041422324fb6f9c2f5f2327e47d5ed264138cb07`  
		Last Modified: Tue, 29 Jun 2021 22:24:21 GMT  
		Size: 316.7 MB (316650088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:beca189572ae6da364127cb9dce2e537e1609513dcfd6aced74c923f0e64a63b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.9 MB (569860363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780c603b8ffad950bda868d810c65006877867052996e76e203c9d9eab5972dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07846d783ec040f65a97338a5da56f9d90ae9459e07dc5cba1fef52c4a6d08d`  
		Last Modified: Wed, 30 Jun 2021 03:11:50 GMT  
		Size: 258.2 MB (258182624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:83f78cf40ffe8dcd158e3cda377c4f4eb6fca675ee7825682a58baeb63129c91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.9 MB (592868141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4e8b7b10ea8ef217b56736521574a6a701fab61c291d82ea79a811b3ba2abf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:03:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9acea9aaf6605dd3b99e32697a815b970bf65d13f7212c9ccce7098b69e3f6`  
		Last Modified: Tue, 29 Jun 2021 22:09:28 GMT  
		Size: 267.2 MB (267223717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:a7f16cf9a61d059c2f655546e7c09a973b5e4d97e54091223599a94535f91ca9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:72a0d008f4bea8fb2c0e0e334f54631a620e16b8c775bd17e1c4b9b7444f2482
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.8 MB (676818460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6a45d8a3e903b25bb7347511fc59162735b9dea255289f8f5d562a293900566`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adac9976a40b77f3bb66a8df041422324fb6f9c2f5f2327e47d5ed264138cb07`  
		Last Modified: Tue, 29 Jun 2021 22:24:21 GMT  
		Size: 316.7 MB (316650088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:beca189572ae6da364127cb9dce2e537e1609513dcfd6aced74c923f0e64a63b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.9 MB (569860363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780c603b8ffad950bda868d810c65006877867052996e76e203c9d9eab5972dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07846d783ec040f65a97338a5da56f9d90ae9459e07dc5cba1fef52c4a6d08d`  
		Last Modified: Wed, 30 Jun 2021 03:11:50 GMT  
		Size: 258.2 MB (258182624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:83f78cf40ffe8dcd158e3cda377c4f4eb6fca675ee7825682a58baeb63129c91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.9 MB (592868141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4e8b7b10ea8ef217b56736521574a6a701fab61c291d82ea79a811b3ba2abf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:03:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9acea9aaf6605dd3b99e32697a815b970bf65d13f7212c9ccce7098b69e3f6`  
		Last Modified: Tue, 29 Jun 2021 22:09:28 GMT  
		Size: 267.2 MB (267223717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:edb985b0b5ffc4989b5af59fb7c2309d4d9daee284030912596b8730d70050f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:1888ec9e88edb5088647c715b7081a15e73d6c28bca3a4442a4371c724d721c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381690263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea5e7f2b8880f6662e39d3768706e5bd24dc55b7411870602bd11384c2a37d53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad556a5f1ba21ba4cc16eabe1f16a36d7610faa1fdf9a483effe3332e086c91`  
		Last Modified: Tue, 29 Jun 2021 22:23:15 GMT  
		Size: 21.5 MB (21521891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:ee42ef07c87e221a64f16d52ae073a535b9f964e272fb4ac07c9c783b78f69f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.0 MB (331954648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c1460e492b3978755c9e8b4a0c0ab0df445da746a6295ecd77fbd38da24247`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:39:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f38543f3bfae9b970c32c7db57152c9cb75781ea5ba68f376e3aa526581ca4`  
		Last Modified: Wed, 30 Jun 2021 03:08:43 GMT  
		Size: 20.3 MB (20276909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cb694e1b3aa2ba0c33ea6ddbc0b17e93f261e58e5751b9d08153c601b0d2268d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.2 MB (346170579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991a0848d36526790f17613eb24904d1a7b13dd7ed6f61ccfb6f4c9f823407a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:02:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29421c42b1d48231a75cd45008b21039f0840d0dffa66badeab06959d8197dc6`  
		Last Modified: Tue, 29 Jun 2021 22:08:27 GMT  
		Size: 20.5 MB (20526155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:edb985b0b5ffc4989b5af59fb7c2309d4d9daee284030912596b8730d70050f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:1888ec9e88edb5088647c715b7081a15e73d6c28bca3a4442a4371c724d721c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381690263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea5e7f2b8880f6662e39d3768706e5bd24dc55b7411870602bd11384c2a37d53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad556a5f1ba21ba4cc16eabe1f16a36d7610faa1fdf9a483effe3332e086c91`  
		Last Modified: Tue, 29 Jun 2021 22:23:15 GMT  
		Size: 21.5 MB (21521891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:ee42ef07c87e221a64f16d52ae073a535b9f964e272fb4ac07c9c783b78f69f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.0 MB (331954648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c1460e492b3978755c9e8b4a0c0ab0df445da746a6295ecd77fbd38da24247`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:39:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f38543f3bfae9b970c32c7db57152c9cb75781ea5ba68f376e3aa526581ca4`  
		Last Modified: Wed, 30 Jun 2021 03:08:43 GMT  
		Size: 20.3 MB (20276909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cb694e1b3aa2ba0c33ea6ddbc0b17e93f261e58e5751b9d08153c601b0d2268d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.2 MB (346170579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991a0848d36526790f17613eb24904d1a7b13dd7ed6f61ccfb6f4c9f823407a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:02:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29421c42b1d48231a75cd45008b21039f0840d0dffa66badeab06959d8197dc6`  
		Last Modified: Tue, 29 Jun 2021 22:08:27 GMT  
		Size: 20.5 MB (20526155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:29c7cb9305475baba4aee5c0b944dca3514c38c9d7b90c5830dfc72ca454ceab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:04f8a0de3d163dbaa208590c46ed4a41445fc78e0074731c29d47b81d28a8506
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.2 MB (360168372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c5711abb297816bcc85d771acaacd9766a66bf679ef9d342e9ef815f158e96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:6aa9871749c213a24f429a77db3f062a7de532602524cd47caf3751794ffb053
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311677739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c7a5e78352deae3cc66bc4c705b3708ce93a311358b919ed921274c9a6ed5ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d412ad704c05401d9fc89b01cfa35678a6b552787b11fa9431a9c2a7619848fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325644424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3dd6b7a1f0ae9bd26af7a0e76f80e51e58ce4756d3e7a8f2dd853f3ea01e28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:29c7cb9305475baba4aee5c0b944dca3514c38c9d7b90c5830dfc72ca454ceab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:04f8a0de3d163dbaa208590c46ed4a41445fc78e0074731c29d47b81d28a8506
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.2 MB (360168372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c5711abb297816bcc85d771acaacd9766a66bf679ef9d342e9ef815f158e96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:11:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:12:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c066b85ea0b10d2eb929bb9007e6c11c3ce86814b523e8f7b4d9d383f206e`  
		Last Modified: Tue, 29 Jun 2021 22:22:55 GMT  
		Size: 57.3 MB (57250492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8274d96e5020c7d93b20123f06998d0683d493e000cb1f1322cf4cd4fcd92f1`  
		Last Modified: Tue, 29 Jun 2021 22:22:44 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea347ac7161f353370e5ce1648f82f7f7c3922584b4847321a24dad27232d4`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 63.6 MB (63575249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:6aa9871749c213a24f429a77db3f062a7de532602524cd47caf3751794ffb053
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311677739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c7a5e78352deae3cc66bc4c705b3708ce93a311358b919ed921274c9a6ed5ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:37:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd25c4b1b9424b6b68be85927855100735e8c39526008685d000c254d01fece`  
		Last Modified: Wed, 30 Jun 2021 03:08:07 GMT  
		Size: 42.9 MB (42895535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4437f32d3366ab514dad754f23ea50bf971bc9a1291f8b23d6d9a60d4e268b`  
		Last Modified: Wed, 30 Jun 2021 03:07:38 GMT  
		Size: 293.7 KB (293731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e630f1a299f7ae71dedf23dcba84039d2424496bb692349b9a914fef972c33c`  
		Last Modified: Wed, 30 Jun 2021 03:08:11 GMT  
		Size: 55.5 MB (55503316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d412ad704c05401d9fc89b01cfa35678a6b552787b11fa9431a9c2a7619848fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325644424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3dd6b7a1f0ae9bd26af7a0e76f80e51e58ce4756d3e7a8f2dd853f3ea01e28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
# Tue, 29 Jun 2021 22:01:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:01:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Jun 2021 22:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df93ae011f7244954c0afa4fae87535aa12db559b169b3fc5723fc5a0e55fe`  
		Last Modified: Tue, 29 Jun 2021 22:08:06 GMT  
		Size: 46.0 MB (45953169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f8a8c40b718f9fcbdac44a9cf459fed379302e6f557fc351cd738fb376e31`  
		Last Modified: Tue, 29 Jun 2021 22:07:58 GMT  
		Size: 293.7 KB (293672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173658f8d064960dbe8f0cc16cddaaa0a9f8e344695c97e0debecf7471cd590`  
		Last Modified: Tue, 29 Jun 2021 22:08:08 GMT  
		Size: 57.3 MB (57297478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:2fe2471dbc1bdc716bcff500fcdc275fd440ef4918c71c5cf64c4db5bb4fa958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:518144280d667d4d39a1faeb6f12c17660a8512481d465284abf35d0534ddfe3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (239048959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d66e4fac4966a3a5ea42ff8380d8612f9f695bb40df1175b9cab63934abadc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:2bf27c4d7af247414dfa948feb54131c5ca8f906d7968ffcea1a22aed61b78c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212985157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afffe9a36c5ca012f47b06ade09be86fbec56c9228e931f9bc8ac792276ef2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bdb0d5f7a8cc3f25d7520cd12ffb30f67e7ce4adfd35dde79b134fbeeb5f2da4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.1 MB (222100105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59af12ff68b67fedfd529212d437fa5431f5eda15825ee64aeeacdf42ba1e75a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:2fe2471dbc1bdc716bcff500fcdc275fd440ef4918c71c5cf64c4db5bb4fa958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:518144280d667d4d39a1faeb6f12c17660a8512481d465284abf35d0534ddfe3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (239048959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d66e4fac4966a3a5ea42ff8380d8612f9f695bb40df1175b9cab63934abadc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:2bf27c4d7af247414dfa948feb54131c5ca8f906d7968ffcea1a22aed61b78c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212985157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afffe9a36c5ca012f47b06ade09be86fbec56c9228e931f9bc8ac792276ef2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bdb0d5f7a8cc3f25d7520cd12ffb30f67e7ce4adfd35dde79b134fbeeb5f2da4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.1 MB (222100105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59af12ff68b67fedfd529212d437fa5431f5eda15825ee64aeeacdf42ba1e75a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:f6cddb1159e664afc1d8b3c556f0dd8fece7ab03a94887cab5e2f977ebb4e397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:b84dc55dec6da1ab52de0b8b11377caa867e9c7d37be12ae66752c2e203f8f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232376681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5459f09fa2f11b0c8d454c2b00df1a21b52549f1af3276dfe4230bb864e03caf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8939446e904c58630b7211dec304744f9f5b26cc0eac113bff1b31f26d85bb46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208507337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107fb98757cb59013e35f1ae50e6cc673dd9da695e44bdb46a0eda65916174ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 01:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:22:12 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:22:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:22:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:22:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93c07c524f5fc3648a3277864f5f70c378f31bf8a69c808daf16881d3e397d3`  
		Last Modified: Fri, 18 Jun 2021 01:40:14 GMT  
		Size: 104.1 MB (104143730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828362a2572407694876df52b6798378f2fcae1b76f01c34d2bf3bcde5431946`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0451cef7bd337ebad4e48e1f3eb634e9417d75ed87155dec3fff664d0fb391`  
		Last Modified: Fri, 18 Jun 2021 01:40:37 GMT  
		Size: 61.0 MB (60970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbc1eed614e6ee80416147df177c36ea5f19940e8b72dc57563513f40822e46`  
		Last Modified: Fri, 18 Jun 2021 01:40:27 GMT  
		Size: 235.2 KB (235206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620e4cae49af2590062e84bff0deb34e1e15c08c2a7a5e37384c230b4b191da`  
		Last Modified: Fri, 18 Jun 2021 01:40:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00222544fae9505236ccdf441360698a6d77df31c78ad609d422651622b07d`  
		Last Modified: Fri, 18 Jun 2021 01:40:29 GMT  
		Size: 9.3 MB (9298549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:bad1a6130b85ab9c4b9df4bc4635ba30d869b2535b8333df5f31e96d4604f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:45f9ae1d29225961cfcc891e8d0ee92d700f4841aa8c8de61b72bbd9a31d594a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437355999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22b9f46caa693f5a476b652bf66e3e545eccebaf4bc37eebe814ec79c8e43d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:7a8aa9f4c0716705e4b542895a010b92179dc5d1bf7f332f849dfb7596eef6e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385865405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6f3e7f4afac45ba8ee5cedd1d70982db4a7f33cf991ba927e87e2a181bbbf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:42bbfb2dfa260b11eca7c2da272cbbd38ba9e4564fc0a63f0d6ca8cf073ef1fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411943994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b25c636fc0740c9410d408ae556841f5df2b94a304085ae6cd20fc12940fc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:22a0d304050d04b7160b85efd5de5b4e47602bf034f7e27d98505fca505e1d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6c94548e7dd7084f82f5a9685c0640c70516584677f11afe37fe8e7f450995a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742475164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deeffb0cbbe69224c3fccf0cb4ddb23fcf493e9912ccef552fb3a93f265c1f66`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793c3e6c7b0812052d8cac51e80bfaf59f0a3ae2a8c2ac432e6c525bd1d6d408`  
		Last Modified: Fri, 18 Jun 2021 02:26:47 GMT  
		Size: 305.1 MB (305119165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:409003e5722b41e90a1400c74e37260ef6cb985cb104b52df6bc9adfe78c9b4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645744854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f304389673ebf992ed4de02bc16101252d8cd7f6fa0d62368f5e3ca704b51155`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:52:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a0fd81acffe6aa873513650ec1943abb8f52f7d8f5ead85dc28a792bf76307`  
		Last Modified: Wed, 30 Jun 2021 03:19:12 GMT  
		Size: 259.9 MB (259879449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1775adc957406b5bcf155d5b70261d9d76578d9b4a0f8aa7c7a6377777bf20c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703398759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a855ce4b2891939ecdcb8b5baeeb12ba0e8d94ca47c0f962d8e051e329280dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56e862e35f4dad2e6104a714b9ab25f30a6953d26af067594e0269d0b8b6dfc`  
		Last Modified: Fri, 18 Jun 2021 01:36:16 GMT  
		Size: 291.5 MB (291454765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:22a0d304050d04b7160b85efd5de5b4e47602bf034f7e27d98505fca505e1d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6c94548e7dd7084f82f5a9685c0640c70516584677f11afe37fe8e7f450995a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742475164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deeffb0cbbe69224c3fccf0cb4ddb23fcf493e9912ccef552fb3a93f265c1f66`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793c3e6c7b0812052d8cac51e80bfaf59f0a3ae2a8c2ac432e6c525bd1d6d408`  
		Last Modified: Fri, 18 Jun 2021 02:26:47 GMT  
		Size: 305.1 MB (305119165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:409003e5722b41e90a1400c74e37260ef6cb985cb104b52df6bc9adfe78c9b4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645744854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f304389673ebf992ed4de02bc16101252d8cd7f6fa0d62368f5e3ca704b51155`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:52:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a0fd81acffe6aa873513650ec1943abb8f52f7d8f5ead85dc28a792bf76307`  
		Last Modified: Wed, 30 Jun 2021 03:19:12 GMT  
		Size: 259.9 MB (259879449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1775adc957406b5bcf155d5b70261d9d76578d9b4a0f8aa7c7a6377777bf20c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703398759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a855ce4b2891939ecdcb8b5baeeb12ba0e8d94ca47c0f962d8e051e329280dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56e862e35f4dad2e6104a714b9ab25f30a6953d26af067594e0269d0b8b6dfc`  
		Last Modified: Fri, 18 Jun 2021 01:36:16 GMT  
		Size: 291.5 MB (291454765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:271a1794a33756d165ef0e9575f746f3709230cbe1716110310d706f5fc293a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:0081d2a47b1008f2f9e6341ec525d9b48ab20218c21f31001fcd583c16763043
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448434037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35978ed9f55ca96736d256b081ae740020d7250016a6b4f948c67489cf80fcc3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840127939fedea917fa03948266ca553ba4ef961388197b323cd4530d7f9c84`  
		Last Modified: Fri, 18 Jun 2021 02:25:40 GMT  
		Size: 11.1 MB (11078038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:db70c713ff0f444bd61eaa7494f65408d1b86881021c3eb1a30993f3af9f106f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395985787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5eb6b3e314e488b74a6ad6f23b0e6275da7417e2edece0d2b5b1c13fcb0eac6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b628a790cd7515455e943c84550f5550c6253f767820dd131edf2466c6e692dd`  
		Last Modified: Wed, 30 Jun 2021 03:16:08 GMT  
		Size: 10.1 MB (10120382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:618890bf1c9e1fc589af0b8a37289145940afd6fb689577c9c5d2371e378d2fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422675404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06888b82cccb9c52119dd61bfae8915ef668145808e717c5c703d1e3222ae36`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18da08529034abf78f8e8545cd98166a3681e28d751ae6cc847c76c0108432dc`  
		Last Modified: Fri, 18 Jun 2021 01:35:08 GMT  
		Size: 10.7 MB (10731410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:271a1794a33756d165ef0e9575f746f3709230cbe1716110310d706f5fc293a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:0081d2a47b1008f2f9e6341ec525d9b48ab20218c21f31001fcd583c16763043
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448434037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35978ed9f55ca96736d256b081ae740020d7250016a6b4f948c67489cf80fcc3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840127939fedea917fa03948266ca553ba4ef961388197b323cd4530d7f9c84`  
		Last Modified: Fri, 18 Jun 2021 02:25:40 GMT  
		Size: 11.1 MB (11078038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:db70c713ff0f444bd61eaa7494f65408d1b86881021c3eb1a30993f3af9f106f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395985787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5eb6b3e314e488b74a6ad6f23b0e6275da7417e2edece0d2b5b1c13fcb0eac6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b628a790cd7515455e943c84550f5550c6253f767820dd131edf2466c6e692dd`  
		Last Modified: Wed, 30 Jun 2021 03:16:08 GMT  
		Size: 10.1 MB (10120382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:618890bf1c9e1fc589af0b8a37289145940afd6fb689577c9c5d2371e378d2fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422675404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06888b82cccb9c52119dd61bfae8915ef668145808e717c5c703d1e3222ae36`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18da08529034abf78f8e8545cd98166a3681e28d751ae6cc847c76c0108432dc`  
		Last Modified: Fri, 18 Jun 2021 01:35:08 GMT  
		Size: 10.7 MB (10731410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:bad1a6130b85ab9c4b9df4bc4635ba30d869b2535b8333df5f31e96d4604f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:45f9ae1d29225961cfcc891e8d0ee92d700f4841aa8c8de61b72bbd9a31d594a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437355999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22b9f46caa693f5a476b652bf66e3e545eccebaf4bc37eebe814ec79c8e43d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:7a8aa9f4c0716705e4b542895a010b92179dc5d1bf7f332f849dfb7596eef6e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385865405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6f3e7f4afac45ba8ee5cedd1d70982db4a7f33cf991ba927e87e2a181bbbf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:42bbfb2dfa260b11eca7c2da272cbbd38ba9e4564fc0a63f0d6ca8cf073ef1fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411943994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b25c636fc0740c9410d408ae556841f5df2b94a304085ae6cd20fc12940fc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:bad1a6130b85ab9c4b9df4bc4635ba30d869b2535b8333df5f31e96d4604f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:45f9ae1d29225961cfcc891e8d0ee92d700f4841aa8c8de61b72bbd9a31d594a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437355999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22b9f46caa693f5a476b652bf66e3e545eccebaf4bc37eebe814ec79c8e43d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:7a8aa9f4c0716705e4b542895a010b92179dc5d1bf7f332f849dfb7596eef6e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385865405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6f3e7f4afac45ba8ee5cedd1d70982db4a7f33cf991ba927e87e2a181bbbf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:42bbfb2dfa260b11eca7c2da272cbbd38ba9e4564fc0a63f0d6ca8cf073ef1fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411943994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b25c636fc0740c9410d408ae556841f5df2b94a304085ae6cd20fc12940fc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:5902ed8e16c7cd74a8cd93bec9379633fd8f577956a6d8a509279a69e80e1754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:245faa8bc7352ccd1fe026976d8207b5afb0f0cbfc84731aa590e6eebf0c6aaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291863614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4e5e7e7b2d86b18740ff9cc42d31e3be1635712bf4b7dec705291aa1a9b688`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:4581069b711c2e438d5a56bb49dd81c070f07e3c76a023f3233fd81c6325caf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266155483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:082cd8fe1b164cc77353db7e188c1965becc24b484222f3201c03766bdd0fe47`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d2b0a7fe9b44edc47d36837369aa42fd069de9e1e6b29623c43def835fddc3fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281396988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99232df8504f400649cbc79aa1194d334b6b38ec29851643bd356b5a9a0b060`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:5902ed8e16c7cd74a8cd93bec9379633fd8f577956a6d8a509279a69e80e1754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:245faa8bc7352ccd1fe026976d8207b5afb0f0cbfc84731aa590e6eebf0c6aaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291863614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4e5e7e7b2d86b18740ff9cc42d31e3be1635712bf4b7dec705291aa1a9b688`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:4581069b711c2e438d5a56bb49dd81c070f07e3c76a023f3233fd81c6325caf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266155483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:082cd8fe1b164cc77353db7e188c1965becc24b484222f3201c03766bdd0fe47`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d2b0a7fe9b44edc47d36837369aa42fd069de9e1e6b29623c43def835fddc3fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281396988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99232df8504f400649cbc79aa1194d334b6b38ec29851643bd356b5a9a0b060`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:3e6a35f079698f09470bf68987e85399dbe6a221322c375406b93dc8cc944e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:c9560582e17e8eed4a72bb18433d1e6f56b70d62513d307993c776bb886d1a78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.9 MB (334891393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950431941162e51c6aa584d795928655524e74288527c44ba2202809e19b0301`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:fde1ae78d99d46536c911daf516f6c0d73352c48869689cac97063169ad93d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285237237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949e9fedc86e0217b5840546b26cb295850dedb52e92f951e1b023ee1f278c0d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2cacf86423c2c0975315fed27525f218224e20bd0872870472187b72b9577a2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314579790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1e70451757ae814799c9bb72e863aa12b8011a49c6049366f2c86e7c86038c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:0364a0ff3169952d12e32bc65e707d39ebd44c15b42d4be5163b3dc814ce73ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:baf62cb6125f2d1713ef45f768a3d2369b25c00540af7baec288d29fba26c479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **834.2 MB (834249484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759ba5e891bacbc11a75049ca91a707a67d70fe2c8d97e3c62ad5ded335495f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce3d94a8d23b1b4e64d7318baa4cab79b3e4f81f1276c72459133910abb6c66`  
		Last Modified: Fri, 18 Jun 2021 02:30:01 GMT  
		Size: 499.4 MB (499358091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:a96c2d1e911db5f317a61d68cd4631bbb7dc61b4c1474aad6496e13c798cdad1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **728.8 MB (728811802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98fa001c88e910512c6a8f998b2688364a10bb10ef9f0694bf18be2ce14e71`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 03:03:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1604ec372f4cb441ab2acab3e66e021bb684ef7ca38ae615855d07ef6d2cc682`  
		Last Modified: Wed, 30 Jun 2021 03:28:08 GMT  
		Size: 443.6 MB (443574565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:57a1d3404eb22282c1311d843ffb1869644db233ccf44f89d29fc027cf239cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **783.2 MB (783206752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114efa1147a4e1b7b13a2de38d2a530e65b230c192042f6386d48bda0e295ea2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42418dcf19529899ebabb4e6fdf8d4ed071bc0a2d300d602986c81b05540dba`  
		Last Modified: Fri, 18 Jun 2021 01:39:31 GMT  
		Size: 468.6 MB (468626962 bytes)  
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
$ docker pull ros@sha256:0364a0ff3169952d12e32bc65e707d39ebd44c15b42d4be5163b3dc814ce73ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:baf62cb6125f2d1713ef45f768a3d2369b25c00540af7baec288d29fba26c479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **834.2 MB (834249484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759ba5e891bacbc11a75049ca91a707a67d70fe2c8d97e3c62ad5ded335495f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce3d94a8d23b1b4e64d7318baa4cab79b3e4f81f1276c72459133910abb6c66`  
		Last Modified: Fri, 18 Jun 2021 02:30:01 GMT  
		Size: 499.4 MB (499358091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:a96c2d1e911db5f317a61d68cd4631bbb7dc61b4c1474aad6496e13c798cdad1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **728.8 MB (728811802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98fa001c88e910512c6a8f998b2688364a10bb10ef9f0694bf18be2ce14e71`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 03:03:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1604ec372f4cb441ab2acab3e66e021bb684ef7ca38ae615855d07ef6d2cc682`  
		Last Modified: Wed, 30 Jun 2021 03:28:08 GMT  
		Size: 443.6 MB (443574565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:57a1d3404eb22282c1311d843ffb1869644db233ccf44f89d29fc027cf239cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **783.2 MB (783206752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114efa1147a4e1b7b13a2de38d2a530e65b230c192042f6386d48bda0e295ea2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42418dcf19529899ebabb4e6fdf8d4ed071bc0a2d300d602986c81b05540dba`  
		Last Modified: Fri, 18 Jun 2021 01:39:31 GMT  
		Size: 468.6 MB (468626962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:8c9e17d392622ad49c63cc1a6dd04aef3eb6c4d773b17ecf01d2324f96e90a1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:cf48a268916b8518806eee81dced07b87bea6f0b9b9953785ccead650f0182ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.6 MB (350627124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:479a373b3df6d1d231b78902ef6e7f419df69295f0a231631ab57579f277a364`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:04:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac135da070f616134577586f204e23c17608bc5538c0c187f4192688a29be8f`  
		Last Modified: Fri, 18 Jun 2021 02:28:22 GMT  
		Size: 15.7 MB (15735731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:886d4ac3ca3d66f0faabe17a6e704b9c9e16e4ae021994bf8d078184fc7c2bef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299197788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f80002eff31e610fb20157f197b2be3ef514c6d1fcc063dc46a994a5d49ce006`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bd942ae3b731cc8abb247f8a202289151d99c372f5c13a11616752c94e0c2b`  
		Last Modified: Wed, 30 Jun 2021 03:23:07 GMT  
		Size: 14.0 MB (13960551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e7c146f828eb03a7b52acec1bc9e060a7324d1da86a96775b98c0b7fb851f56a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329930712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e68c2ffa7ce5e4e0af76f581e3af96e441d58609a8494f2384496053acbdcbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f2e8446ad97b3f05d8a909bc1a80a970cd634e819edac7e15c1c969c68f0dc`  
		Last Modified: Fri, 18 Jun 2021 01:37:53 GMT  
		Size: 15.4 MB (15350922 bytes)  
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
$ docker pull ros@sha256:8c9e17d392622ad49c63cc1a6dd04aef3eb6c4d773b17ecf01d2324f96e90a1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:cf48a268916b8518806eee81dced07b87bea6f0b9b9953785ccead650f0182ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.6 MB (350627124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:479a373b3df6d1d231b78902ef6e7f419df69295f0a231631ab57579f277a364`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:04:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac135da070f616134577586f204e23c17608bc5538c0c187f4192688a29be8f`  
		Last Modified: Fri, 18 Jun 2021 02:28:22 GMT  
		Size: 15.7 MB (15735731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:886d4ac3ca3d66f0faabe17a6e704b9c9e16e4ae021994bf8d078184fc7c2bef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299197788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f80002eff31e610fb20157f197b2be3ef514c6d1fcc063dc46a994a5d49ce006`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bd942ae3b731cc8abb247f8a202289151d99c372f5c13a11616752c94e0c2b`  
		Last Modified: Wed, 30 Jun 2021 03:23:07 GMT  
		Size: 14.0 MB (13960551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e7c146f828eb03a7b52acec1bc9e060a7324d1da86a96775b98c0b7fb851f56a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329930712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e68c2ffa7ce5e4e0af76f581e3af96e441d58609a8494f2384496053acbdcbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f2e8446ad97b3f05d8a909bc1a80a970cd634e819edac7e15c1c969c68f0dc`  
		Last Modified: Fri, 18 Jun 2021 01:37:53 GMT  
		Size: 15.4 MB (15350922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:3e6a35f079698f09470bf68987e85399dbe6a221322c375406b93dc8cc944e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c9560582e17e8eed4a72bb18433d1e6f56b70d62513d307993c776bb886d1a78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.9 MB (334891393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950431941162e51c6aa584d795928655524e74288527c44ba2202809e19b0301`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:fde1ae78d99d46536c911daf516f6c0d73352c48869689cac97063169ad93d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285237237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949e9fedc86e0217b5840546b26cb295850dedb52e92f951e1b023ee1f278c0d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2cacf86423c2c0975315fed27525f218224e20bd0872870472187b72b9577a2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314579790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1e70451757ae814799c9bb72e863aa12b8011a49c6049366f2c86e7c86038c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
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
$ docker pull ros@sha256:3e6a35f079698f09470bf68987e85399dbe6a221322c375406b93dc8cc944e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:c9560582e17e8eed4a72bb18433d1e6f56b70d62513d307993c776bb886d1a78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.9 MB (334891393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950431941162e51c6aa584d795928655524e74288527c44ba2202809e19b0301`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:fde1ae78d99d46536c911daf516f6c0d73352c48869689cac97063169ad93d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285237237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949e9fedc86e0217b5840546b26cb295850dedb52e92f951e1b023ee1f278c0d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2cacf86423c2c0975315fed27525f218224e20bd0872870472187b72b9577a2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314579790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1e70451757ae814799c9bb72e863aa12b8011a49c6049366f2c86e7c86038c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:9187690fa6ac249b04783e888b39049796e973e2e09911f4e5204c7ba71de5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:1941de6f440620aa7b6bea5fd91a59e5bc6c8797f6608d9d6a7b478f67e5cf1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208598020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7af942b15c8cce5753a48a27d95573545e4e910bda4840278c8de005bc222ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:2ce7bdf48270fce12b2a3b752b62dc24245c28a50f435fe553153a0aab3ec3c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187753564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf2df904864e2bc2df14f7effce20a88088554318ca9574dc23c5e5342d11f8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d864de892ce59ee974de53c0b5671b23b669609a29b4a6d1298f4e15828a8c30
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.6 MB (201649162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abbeb1b6b1198ddf434b32883501980337d6997a48d4902e91415ca3eb333cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
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
$ docker pull ros@sha256:9187690fa6ac249b04783e888b39049796e973e2e09911f4e5204c7ba71de5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:1941de6f440620aa7b6bea5fd91a59e5bc6c8797f6608d9d6a7b478f67e5cf1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208598020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7af942b15c8cce5753a48a27d95573545e4e910bda4840278c8de005bc222ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:2ce7bdf48270fce12b2a3b752b62dc24245c28a50f435fe553153a0aab3ec3c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187753564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf2df904864e2bc2df14f7effce20a88088554318ca9574dc23c5e5342d11f8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d864de892ce59ee974de53c0b5671b23b669609a29b4a6d1298f4e15828a8c30
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.6 MB (201649162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abbeb1b6b1198ddf434b32883501980337d6997a48d4902e91415ca3eb333cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:4d0de0fedcd4d538a2062295baa8ec5d3e556d709fe8f925e3abbc45812dbe03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:38ddc87677cc7bafa7e79d4537365db18e9a870ebe35e51cd27274934c4723f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227799414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f840f83bd31e9a5d7d9b295c6b3fda49a0c27d1ec885e94ca6e4035b6c7aa286`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:19:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:19:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837448df0815a613ee720a81c9f44ab668e5e4b2b2616b6f31a4495fea465839`  
		Last Modified: Fri, 18 Jun 2021 02:34:23 GMT  
		Size: 66.6 MB (66550472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420cde9136fdf7d018e6571536582bd69834d41d6f368fb1c18b4c250c02bcf`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 233.9 KB (233906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4da8004060a34a319a474c460b80e1554f49287d7b0f6caed1ad1fe56fc325`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7a80f8badad65537ffae8798f29e730fa7544eec2776c97651295d0f70f5c`  
		Last Modified: Fri, 18 Jun 2021 02:34:16 GMT  
		Size: 22.1 MB (22112431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:36978ae0d71bc97c87a1d7016666891834070cb32ae40b1e2998f250609f71dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216458936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc18d05437376ebbf497d2a619da7455990100e5e0dbabe08c401422737e9f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:27:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:27:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:27:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e76e8ff735e23ef93c1cf44e242fedcb3b6e64a4b2a997c805c35bcee5c873`  
		Last Modified: Fri, 18 Jun 2021 01:43:59 GMT  
		Size: 60.9 MB (60920414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1df38f1e163e319dd6129117780d6180bc8da2a601e74b550af1d5befff34e`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 233.9 KB (233901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb6fb4d817acd74ea55098bd6e036e4b5209499d19354e72daba5f51c9b3a8`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410e6c24794ec3018d5effc08528698df0ff5573a7a3b39e14ce6de24e2f9c1d`  
		Last Modified: Fri, 18 Jun 2021 01:43:51 GMT  
		Size: 21.4 MB (21449057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:4d0de0fedcd4d538a2062295baa8ec5d3e556d709fe8f925e3abbc45812dbe03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:38ddc87677cc7bafa7e79d4537365db18e9a870ebe35e51cd27274934c4723f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227799414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f840f83bd31e9a5d7d9b295c6b3fda49a0c27d1ec885e94ca6e4035b6c7aa286`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:19:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:19:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837448df0815a613ee720a81c9f44ab668e5e4b2b2616b6f31a4495fea465839`  
		Last Modified: Fri, 18 Jun 2021 02:34:23 GMT  
		Size: 66.6 MB (66550472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420cde9136fdf7d018e6571536582bd69834d41d6f368fb1c18b4c250c02bcf`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 233.9 KB (233906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4da8004060a34a319a474c460b80e1554f49287d7b0f6caed1ad1fe56fc325`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7a80f8badad65537ffae8798f29e730fa7544eec2776c97651295d0f70f5c`  
		Last Modified: Fri, 18 Jun 2021 02:34:16 GMT  
		Size: 22.1 MB (22112431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:36978ae0d71bc97c87a1d7016666891834070cb32ae40b1e2998f250609f71dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216458936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc18d05437376ebbf497d2a619da7455990100e5e0dbabe08c401422737e9f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:27:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:27:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:27:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e76e8ff735e23ef93c1cf44e242fedcb3b6e64a4b2a997c805c35bcee5c873`  
		Last Modified: Fri, 18 Jun 2021 01:43:59 GMT  
		Size: 60.9 MB (60920414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1df38f1e163e319dd6129117780d6180bc8da2a601e74b550af1d5befff34e`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 233.9 KB (233901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb6fb4d817acd74ea55098bd6e036e4b5209499d19354e72daba5f51c9b3a8`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410e6c24794ec3018d5effc08528698df0ff5573a7a3b39e14ce6de24e2f9c1d`  
		Last Modified: Fri, 18 Jun 2021 01:43:51 GMT  
		Size: 21.4 MB (21449057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:4d0de0fedcd4d538a2062295baa8ec5d3e556d709fe8f925e3abbc45812dbe03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:38ddc87677cc7bafa7e79d4537365db18e9a870ebe35e51cd27274934c4723f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227799414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f840f83bd31e9a5d7d9b295c6b3fda49a0c27d1ec885e94ca6e4035b6c7aa286`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:19:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:19:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837448df0815a613ee720a81c9f44ab668e5e4b2b2616b6f31a4495fea465839`  
		Last Modified: Fri, 18 Jun 2021 02:34:23 GMT  
		Size: 66.6 MB (66550472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420cde9136fdf7d018e6571536582bd69834d41d6f368fb1c18b4c250c02bcf`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 233.9 KB (233906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4da8004060a34a319a474c460b80e1554f49287d7b0f6caed1ad1fe56fc325`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7a80f8badad65537ffae8798f29e730fa7544eec2776c97651295d0f70f5c`  
		Last Modified: Fri, 18 Jun 2021 02:34:16 GMT  
		Size: 22.1 MB (22112431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:36978ae0d71bc97c87a1d7016666891834070cb32ae40b1e2998f250609f71dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216458936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc18d05437376ebbf497d2a619da7455990100e5e0dbabe08c401422737e9f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:27:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:27:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:27:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e76e8ff735e23ef93c1cf44e242fedcb3b6e64a4b2a997c805c35bcee5c873`  
		Last Modified: Fri, 18 Jun 2021 01:43:59 GMT  
		Size: 60.9 MB (60920414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1df38f1e163e319dd6129117780d6180bc8da2a601e74b550af1d5befff34e`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 233.9 KB (233901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb6fb4d817acd74ea55098bd6e036e4b5209499d19354e72daba5f51c9b3a8`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410e6c24794ec3018d5effc08528698df0ff5573a7a3b39e14ce6de24e2f9c1d`  
		Last Modified: Fri, 18 Jun 2021 01:43:51 GMT  
		Size: 21.4 MB (21449057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:cb2b86fbd465545483628f1e5a3c9f61b7b4d7cb2d99dbd248193ffd60681b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:6fd5833b85783db7ab6fc4811ad6aaadc003c1be1d676709250fa03b1b0ab5e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138900573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd0b86b5088297c9c962f4350fec182cb37c8c3a62dd5e45ff3c6da5bae698c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4fe1e8027217eb90657af6bfbf104b4fcfe31c3a9d0d643fe163ab57816703f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133853517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea97e65bb7274da9f4cc078271c1793d29eed4d29cf94f4ab50eb82d8a550f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-focal`

```console
$ docker pull ros@sha256:cb2b86fbd465545483628f1e5a3c9f61b7b4d7cb2d99dbd248193ffd60681b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6fd5833b85783db7ab6fc4811ad6aaadc003c1be1d676709250fa03b1b0ab5e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138900573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd0b86b5088297c9c962f4350fec182cb37c8c3a62dd5e45ff3c6da5bae698c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4fe1e8027217eb90657af6bfbf104b4fcfe31c3a9d0d643fe163ab57816703f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133853517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea97e65bb7274da9f4cc078271c1793d29eed4d29cf94f4ab50eb82d8a550f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:98161e62b6d4d01e905c45deae895fa0092d830bfe75eab6c1706b9e8c30748f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:f3eda3ea6e4b097bb2c8f08eef1d804c64f486d76fe70a16dbc9566bdd2b9287
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321262923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299aed0c28d698fc0d30005feebaeb19c4db40a65a8bfda5077a585b904223eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:19:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:19:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:19:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:19:49 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:19:49 GMT
ENV ROS2_DISTRO=rolling
# Fri, 18 Jun 2021 02:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:20:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:20:26 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837448df0815a613ee720a81c9f44ab668e5e4b2b2616b6f31a4495fea465839`  
		Last Modified: Fri, 18 Jun 2021 02:34:23 GMT  
		Size: 66.6 MB (66550472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420cde9136fdf7d018e6571536582bd69834d41d6f368fb1c18b4c250c02bcf`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 233.9 KB (233906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4da8004060a34a319a474c460b80e1554f49287d7b0f6caed1ad1fe56fc325`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7a80f8badad65537ffae8798f29e730fa7544eec2776c97651295d0f70f5c`  
		Last Modified: Fri, 18 Jun 2021 02:34:16 GMT  
		Size: 22.1 MB (22112431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2223c216945e3173e68c2c7a500219b338b0cd99698a843ac182d2775a79898`  
		Last Modified: Fri, 18 Jun 2021 02:34:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe759e8c92b56e706d56bc8d57690f6a4c9f4be6441d8914bffc122167b2a3d`  
		Last Modified: Fri, 18 Jun 2021 02:34:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d2347f07e71fe05985b3ec49b07db5a4c527e8d8c3cd1b7ccf82226b6db9b9`  
		Last Modified: Fri, 18 Jun 2021 02:34:59 GMT  
		Size: 78.4 MB (78410443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231e643896b536ffd9b3195c3de2991757e06005c986cd264a221f188ae89151`  
		Last Modified: Fri, 18 Jun 2021 02:34:42 GMT  
		Size: 15.1 MB (15052441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe5a309ec844c860dcdc4d2ee8cc0bfd97bf10184a7a762c0d998af43f4f5af`  
		Last Modified: Fri, 18 Jun 2021 02:34:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:509721406f962fda338a96d93880cdff5332e1af6194561d73e812fb46ca29c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.5 MB (309458223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a17bf27ac7c4419c7678c486093312b7122f73f9116b037f0667f85f9910d10e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:27:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:27:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:27:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:28:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:28:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:28:08 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 01:28:09 GMT
ENV ROS2_DISTRO=rolling
# Fri, 18 Jun 2021 01:28:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:28:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:28:44 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e76e8ff735e23ef93c1cf44e242fedcb3b6e64a4b2a997c805c35bcee5c873`  
		Last Modified: Fri, 18 Jun 2021 01:43:59 GMT  
		Size: 60.9 MB (60920414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1df38f1e163e319dd6129117780d6180bc8da2a601e74b550af1d5befff34e`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 233.9 KB (233901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb6fb4d817acd74ea55098bd6e036e4b5209499d19354e72daba5f51c9b3a8`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410e6c24794ec3018d5effc08528698df0ff5573a7a3b39e14ce6de24e2f9c1d`  
		Last Modified: Fri, 18 Jun 2021 01:43:51 GMT  
		Size: 21.4 MB (21449057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c88ab0e230b56f3d70dc8bd6086185f33c6cf8691e3636ab1aa8ed3ee20bb9e`  
		Last Modified: Fri, 18 Jun 2021 01:44:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75033272b9606e67db1d30b41ca9ff4ec77d2202ea1f45a4af8c72fb455b26d`  
		Last Modified: Fri, 18 Jun 2021 01:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd74012273e262686f50ee17beb69b592dbde8e21ba7950482664641b4b0a8e`  
		Last Modified: Fri, 18 Jun 2021 01:44:33 GMT  
		Size: 78.4 MB (78368152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a9e437753adba152a9f605e3a44baf39ca2168ebbf1b7532a7601a3125ede`  
		Last Modified: Fri, 18 Jun 2021 01:44:19 GMT  
		Size: 14.6 MB (14630507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84555ec2e7115b410ff325e240f2acdc36d84ab16e73f226675800fb3f09c356`  
		Last Modified: Fri, 18 Jun 2021 01:44:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:98161e62b6d4d01e905c45deae895fa0092d830bfe75eab6c1706b9e8c30748f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:f3eda3ea6e4b097bb2c8f08eef1d804c64f486d76fe70a16dbc9566bdd2b9287
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321262923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299aed0c28d698fc0d30005feebaeb19c4db40a65a8bfda5077a585b904223eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:19:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:19:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:19:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:19:49 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:19:49 GMT
ENV ROS2_DISTRO=rolling
# Fri, 18 Jun 2021 02:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:20:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:20:26 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837448df0815a613ee720a81c9f44ab668e5e4b2b2616b6f31a4495fea465839`  
		Last Modified: Fri, 18 Jun 2021 02:34:23 GMT  
		Size: 66.6 MB (66550472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420cde9136fdf7d018e6571536582bd69834d41d6f368fb1c18b4c250c02bcf`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 233.9 KB (233906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4da8004060a34a319a474c460b80e1554f49287d7b0f6caed1ad1fe56fc325`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7a80f8badad65537ffae8798f29e730fa7544eec2776c97651295d0f70f5c`  
		Last Modified: Fri, 18 Jun 2021 02:34:16 GMT  
		Size: 22.1 MB (22112431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2223c216945e3173e68c2c7a500219b338b0cd99698a843ac182d2775a79898`  
		Last Modified: Fri, 18 Jun 2021 02:34:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe759e8c92b56e706d56bc8d57690f6a4c9f4be6441d8914bffc122167b2a3d`  
		Last Modified: Fri, 18 Jun 2021 02:34:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d2347f07e71fe05985b3ec49b07db5a4c527e8d8c3cd1b7ccf82226b6db9b9`  
		Last Modified: Fri, 18 Jun 2021 02:34:59 GMT  
		Size: 78.4 MB (78410443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231e643896b536ffd9b3195c3de2991757e06005c986cd264a221f188ae89151`  
		Last Modified: Fri, 18 Jun 2021 02:34:42 GMT  
		Size: 15.1 MB (15052441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe5a309ec844c860dcdc4d2ee8cc0bfd97bf10184a7a762c0d998af43f4f5af`  
		Last Modified: Fri, 18 Jun 2021 02:34:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:509721406f962fda338a96d93880cdff5332e1af6194561d73e812fb46ca29c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.5 MB (309458223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a17bf27ac7c4419c7678c486093312b7122f73f9116b037f0667f85f9910d10e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:21:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 01:21:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:21:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:26:23 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 01:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 01:27:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:27:04 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:27:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:27:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:27:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 01:27:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:28:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:28:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:28:08 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 01:28:09 GMT
ENV ROS2_DISTRO=rolling
# Fri, 18 Jun 2021 01:28:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:28:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:28:44 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5209be94969f98c26b06c264ea08cf71bb1283c69ce7ca685f96e270e387d3`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba4e54c2e10d6e40ec38a204350abcbb7acc2e9d1756e4cfdf8ed8ac35161a`  
		Last Modified: Fri, 18 Jun 2021 01:39:51 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bab0643538a88d3237e1034009da28994975922425be6c79e06599667902ec`  
		Last Modified: Fri, 18 Jun 2021 01:43:30 GMT  
		Size: 100.0 MB (99995784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa4adc2b9dbbabfbe5de417d9c78e594674a4073380274bdc09509b6a717a4`  
		Last Modified: Fri, 18 Jun 2021 01:43:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e76e8ff735e23ef93c1cf44e242fedcb3b6e64a4b2a997c805c35bcee5c873`  
		Last Modified: Fri, 18 Jun 2021 01:43:59 GMT  
		Size: 60.9 MB (60920414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1df38f1e163e319dd6129117780d6180bc8da2a601e74b550af1d5befff34e`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 233.9 KB (233901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb6fb4d817acd74ea55098bd6e036e4b5209499d19354e72daba5f51c9b3a8`  
		Last Modified: Fri, 18 Jun 2021 01:43:47 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410e6c24794ec3018d5effc08528698df0ff5573a7a3b39e14ce6de24e2f9c1d`  
		Last Modified: Fri, 18 Jun 2021 01:43:51 GMT  
		Size: 21.4 MB (21449057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c88ab0e230b56f3d70dc8bd6086185f33c6cf8691e3636ab1aa8ed3ee20bb9e`  
		Last Modified: Fri, 18 Jun 2021 01:44:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75033272b9606e67db1d30b41ca9ff4ec77d2202ea1f45a4af8c72fb455b26d`  
		Last Modified: Fri, 18 Jun 2021 01:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd74012273e262686f50ee17beb69b592dbde8e21ba7950482664641b4b0a8e`  
		Last Modified: Fri, 18 Jun 2021 01:44:33 GMT  
		Size: 78.4 MB (78368152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a9e437753adba152a9f605e3a44baf39ca2168ebbf1b7532a7601a3125ede`  
		Last Modified: Fri, 18 Jun 2021 01:44:19 GMT  
		Size: 14.6 MB (14630507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84555ec2e7115b410ff325e240f2acdc36d84ab16e73f226675800fb3f09c356`  
		Last Modified: Fri, 18 Jun 2021 01:44:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
