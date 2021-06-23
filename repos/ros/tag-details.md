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
$ docker pull ros@sha256:636ce2f45e378a94defeb7018eaf56f36fc436c84b034f8f911f3dd833f1279f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:93a496e827d067811ba72da0f484a6a3d14930e4f9989ec2b38df8b9cc0eec8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.2 MB (360158904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de84e9adf03c169a1f98474a23d53f64488f9850d25b565fa8ea5ebf62e62ec3`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3514be578da03c4dae04da89772514ce66ebb45680157843aa74927236bb2f07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311669266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b3f2625f655d8f2dcde3d4508d2825c9cda5df1613740cc93b479b0980ff45`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:09b05820d670dc4a265f6dcc4f643ce4fc33949fc364725a8de6d0248882665c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325640560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb793f4cd7b170dd3ef8d9a40eba73da2010db223506a5b4cd96ab048e662512`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:3ae160b5d6e89be1955b9e106643314ca5d147924ef949556497552596c7762e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:8dab97a8da9216567925c76527730756776d5831ae148c34dfb18a8e2cc401f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.8 MB (676809293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87555f7af7f012664b7c3c592348b44cddeb678d1c10f132a446d5c29871d268`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:42:30 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebb911d36564f36933f5d4d1b7f8cd40385d068603a9d6cf9e39c7899e16bfc`  
		Last Modified: Fri, 18 Jun 2021 02:23:54 GMT  
		Size: 316.7 MB (316650389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:3489339110d0d58e8aab0b31fb7a82768b3b5275731f9418676275bae7727c61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.8 MB (569849897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:074a57488c85c601bea021b94a706cdebb9b49115ff61c3f983e7c27a3f4f2bb`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:33:43 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91c3c27ab8c8da0e782cf994e545cc252a5fb19378c1b70f55938f8bf2a7bb4`  
		Last Modified: Fri, 18 Jun 2021 00:48:10 GMT  
		Size: 258.2 MB (258180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fe044f4f95ee915afa881b134aee3a72adb986c05bed4479fde7729d47533394
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.9 MB (592864080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:106f6414cd7ccd4251dbd848e226e5a32fb1abda58198a43ee073d1a9cfb6d8d`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:08 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6927a1ee2abcb2fa7c24390b1bb1516339313282c2257add2375e42365e8dd`  
		Last Modified: Fri, 18 Jun 2021 01:33:15 GMT  
		Size: 267.2 MB (267223520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:3ae160b5d6e89be1955b9e106643314ca5d147924ef949556497552596c7762e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:8dab97a8da9216567925c76527730756776d5831ae148c34dfb18a8e2cc401f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.8 MB (676809293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87555f7af7f012664b7c3c592348b44cddeb678d1c10f132a446d5c29871d268`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:42:30 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebb911d36564f36933f5d4d1b7f8cd40385d068603a9d6cf9e39c7899e16bfc`  
		Last Modified: Fri, 18 Jun 2021 02:23:54 GMT  
		Size: 316.7 MB (316650389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:3489339110d0d58e8aab0b31fb7a82768b3b5275731f9418676275bae7727c61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.8 MB (569849897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:074a57488c85c601bea021b94a706cdebb9b49115ff61c3f983e7c27a3f4f2bb`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:33:43 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91c3c27ab8c8da0e782cf994e545cc252a5fb19378c1b70f55938f8bf2a7bb4`  
		Last Modified: Fri, 18 Jun 2021 00:48:10 GMT  
		Size: 258.2 MB (258180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fe044f4f95ee915afa881b134aee3a72adb986c05bed4479fde7729d47533394
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.9 MB (592864080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:106f6414cd7ccd4251dbd848e226e5a32fb1abda58198a43ee073d1a9cfb6d8d`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:08 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6927a1ee2abcb2fa7c24390b1bb1516339313282c2257add2375e42365e8dd`  
		Last Modified: Fri, 18 Jun 2021 01:33:15 GMT  
		Size: 267.2 MB (267223520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:1717521ba91f267c549273ca813d83fc7b9c1728ccc474e5805821c9289d02f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:1183de299a296641248f7b0db38bbe6585b426c93750f2c80d9a8fb1349a2353
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381680736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99feee768b3c1e2d7f68078cf16a1cf676ff29d300098b66b88fbf35f935b3f`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:39:49 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7f06dee01c4ec1a706f93cc4b52fe035110a64966520fd43d0ac140d7a28f`  
		Last Modified: Fri, 18 Jun 2021 02:22:45 GMT  
		Size: 21.5 MB (21521832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:706106d7df6387196bcdbc098cd78c51aefd41e2756ab1334ee70412a3015136
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331945578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cad7fc8c04dca9d6f5f272282c987f37e238dbb33b3210a71e0a65185fe1b31`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:32:20 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc54f0ac7f2d8025a345e3016d775d2f52d5f9ad1eb177d3c47696c521d68925`  
		Last Modified: Fri, 18 Jun 2021 00:47:05 GMT  
		Size: 20.3 MB (20276312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f58ad98eed4789fa4917d7dd9fb0356872d183e156b8d244a81e87dbca415910
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.2 MB (346166612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e629ef390dd69385a761e0e77872c7b1c531374922b079b3194a73b6b90154`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:57 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5bb1b486bb11912526fc0d6db09d7cf486b366916b74b1916d0316e1771114`  
		Last Modified: Fri, 18 Jun 2021 01:32:10 GMT  
		Size: 20.5 MB (20526052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:1717521ba91f267c549273ca813d83fc7b9c1728ccc474e5805821c9289d02f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:1183de299a296641248f7b0db38bbe6585b426c93750f2c80d9a8fb1349a2353
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381680736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99feee768b3c1e2d7f68078cf16a1cf676ff29d300098b66b88fbf35f935b3f`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:39:49 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7f06dee01c4ec1a706f93cc4b52fe035110a64966520fd43d0ac140d7a28f`  
		Last Modified: Fri, 18 Jun 2021 02:22:45 GMT  
		Size: 21.5 MB (21521832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:706106d7df6387196bcdbc098cd78c51aefd41e2756ab1334ee70412a3015136
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331945578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cad7fc8c04dca9d6f5f272282c987f37e238dbb33b3210a71e0a65185fe1b31`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:32:20 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc54f0ac7f2d8025a345e3016d775d2f52d5f9ad1eb177d3c47696c521d68925`  
		Last Modified: Fri, 18 Jun 2021 00:47:05 GMT  
		Size: 20.3 MB (20276312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f58ad98eed4789fa4917d7dd9fb0356872d183e156b8d244a81e87dbca415910
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.2 MB (346166612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e629ef390dd69385a761e0e77872c7b1c531374922b079b3194a73b6b90154`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:57 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5bb1b486bb11912526fc0d6db09d7cf486b366916b74b1916d0316e1771114`  
		Last Modified: Fri, 18 Jun 2021 01:32:10 GMT  
		Size: 20.5 MB (20526052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:636ce2f45e378a94defeb7018eaf56f36fc436c84b034f8f911f3dd833f1279f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:93a496e827d067811ba72da0f484a6a3d14930e4f9989ec2b38df8b9cc0eec8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.2 MB (360158904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de84e9adf03c169a1f98474a23d53f64488f9850d25b565fa8ea5ebf62e62ec3`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:3514be578da03c4dae04da89772514ce66ebb45680157843aa74927236bb2f07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311669266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b3f2625f655d8f2dcde3d4508d2825c9cda5df1613740cc93b479b0980ff45`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:09b05820d670dc4a265f6dcc4f643ce4fc33949fc364725a8de6d0248882665c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325640560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb793f4cd7b170dd3ef8d9a40eba73da2010db223506a5b4cd96ab048e662512`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:636ce2f45e378a94defeb7018eaf56f36fc436c84b034f8f911f3dd833f1279f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:93a496e827d067811ba72da0f484a6a3d14930e4f9989ec2b38df8b9cc0eec8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.2 MB (360158904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de84e9adf03c169a1f98474a23d53f64488f9850d25b565fa8ea5ebf62e62ec3`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:38:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:38:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:39:13 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec23c64ab5c7890c60f3e104df58d70f818a843277b74ca16e0dc07013955`  
		Last Modified: Fri, 18 Jun 2021 02:22:24 GMT  
		Size: 57.3 MB (57250445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88bc24d70588b116ae88f6966a6a202f306d9b1a988deac2d177d083b2da7bc`  
		Last Modified: Fri, 18 Jun 2021 02:22:14 GMT  
		Size: 293.1 KB (293144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257fbf5f818f022eadb79421d2d94b22361a983a18a4578be8ba508cb0392c0`  
		Last Modified: Fri, 18 Jun 2021 02:22:26 GMT  
		Size: 63.6 MB (63575994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:3514be578da03c4dae04da89772514ce66ebb45680157843aa74927236bb2f07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311669266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b3f2625f655d8f2dcde3d4508d2825c9cda5df1613740cc93b479b0980ff45`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:31:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:31:53 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7072639f5c50d212ecab0d5ca3145790aa875e642fd60fbd879f2aa534da5`  
		Last Modified: Fri, 18 Jun 2021 00:46:39 GMT  
		Size: 42.9 MB (42894646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb378cb5724d93bd55641fed615e4b4566eda5100a5c87351ef984eead43bd`  
		Last Modified: Fri, 18 Jun 2021 00:46:31 GMT  
		Size: 293.2 KB (293166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc747c100009636799f3daaa7f5f7fb1200075cab4c30e48e73b31431f045ddc`  
		Last Modified: Fri, 18 Jun 2021 00:46:42 GMT  
		Size: 55.5 MB (55501753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:09b05820d670dc4a265f6dcc4f643ce4fc33949fc364725a8de6d0248882665c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325640560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb793f4cd7b170dd3ef8d9a40eba73da2010db223506a5b4cd96ab048e662512`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:10:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:10:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:10:37 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4501fb1e4cd87f53e7a8521f086c0b97e7a8ef2cad72e5bc3c2451e60a2aaaa`  
		Last Modified: Fri, 18 Jun 2021 01:31:46 GMT  
		Size: 46.0 MB (45953207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704173447f2d9215e352c7a94ab1b4f74076c8ef610d00b584e036a0c3a10ed7`  
		Last Modified: Fri, 18 Jun 2021 01:31:39 GMT  
		Size: 293.1 KB (293147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc12bdc4eaaabdc09276e817282b107e4fd13c106239317845f9399c92c38459`  
		Last Modified: Fri, 18 Jun 2021 01:31:49 GMT  
		Size: 57.3 MB (57297149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:3ca3131c054de2bf732fede94d8f0bf7d8b4f405d97e1a2822d03afd6038e1b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:bfb11a36ee700b39e2a353418b9254163e3ab470752a620f82ec0e49374d1fd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (239039321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704ef0c47b6c270ebc61186f22bc15d289b127d19b3f189b3de806ae5e068daa`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:38fbb5c633fb11dbfccc6269bacceac38ced36de1b29930d8c52dea53c5bfd72
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212979701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1552fc8eebee9145d2c6494f6aec7dc134e247691703fca429b84e5ab55ba0cb`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3587b74788bf13cbddfc0f210946477789036588a455547452cb8e54e26e084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.1 MB (222097057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:637cd8c66245ba3998481fa50761cf62ea2b6a6287150b36bbcb349edc46b545`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:3ca3131c054de2bf732fede94d8f0bf7d8b4f405d97e1a2822d03afd6038e1b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:bfb11a36ee700b39e2a353418b9254163e3ab470752a620f82ec0e49374d1fd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (239039321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704ef0c47b6c270ebc61186f22bc15d289b127d19b3f189b3de806ae5e068daa`
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
# Fri, 18 Jun 2021 01:36:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:36:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:36:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:37:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:37:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:37:56 GMT
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
	-	`sha256:07dea51cd413c41fe30940f98c9baa08e19ec842e9f047b9aca8e4cff5594cbf`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d10f41c924f2a8459161d7db16e0657b6c3fca53699a511a34e7d41b0df092`  
		Last Modified: Fri, 18 Jun 2021 02:21:22 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1d8faebb89e33cd353f0212c76e77bbffd7f078890661ce66d648965b3d203`  
		Last Modified: Fri, 18 Jun 2021 02:22:03 GMT  
		Size: 187.2 MB (187160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21703352205d9f4266473491592b343f90e15750898a6b4756df99776a075241`  
		Last Modified: Fri, 18 Jun 2021 02:21:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:38fbb5c633fb11dbfccc6269bacceac38ced36de1b29930d8c52dea53c5bfd72
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212979701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1552fc8eebee9145d2c6494f6aec7dc134e247691703fca429b84e5ab55ba0cb`
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
# Fri, 18 Jun 2021 00:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:29:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:29:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:29:48 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 00:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:30:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:30:53 GMT
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
	-	`sha256:5930f6d7c7ccb8bd3795bd0d94af884f0a9f95c6b699e47ebf41c41e3001a858`  
		Last Modified: Fri, 18 Jun 2021 00:45:34 GMT  
		Size: 4.6 MB (4615682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c89ce215aaca078da4221c4d14714d8cd4134d2aeec0c05e3ce3af98c55c037`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ddb7cdf85392eba956848eb9f90f6cd0ca3a1b90cf3f279547a64be4ae34c`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 15.3 KB (15292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2dcfe56a94dffc7fde73d7ac3536506f30a2f8ea201701cd36d414c965319`  
		Last Modified: Fri, 18 Jun 2021 00:46:17 GMT  
		Size: 168.0 MB (168034337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572520c93feba7cb3ee2b4b1a8ed6de5c311bd81f582c33f73507653a1e4603`  
		Last Modified: Fri, 18 Jun 2021 00:45:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3587b74788bf13cbddfc0f210946477789036588a455547452cb8e54e26e084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.1 MB (222097057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:637cd8c66245ba3998481fa50761cf62ea2b6a6287150b36bbcb349edc46b545`
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
# Fri, 18 Jun 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:08:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:08:49 GMT
ENV ROS_DISTRO=kinetic
# Fri, 18 Jun 2021 01:09:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:09:46 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:09:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:09:47 GMT
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
	-	`sha256:2b73a6369b56463a3ab8668ab07fc1ae8aa54551838987cf3acd46f7dae243c6`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90311091e07444c6bec45b5ecce522ae94d527d4350d05e21bd3479911613a`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 15.3 KB (15293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add027dfbb07933e127e94649626c0d2c6696337cdf8eea05e781db7e9face50`  
		Last Modified: Fri, 18 Jun 2021 01:31:22 GMT  
		Size: 176.0 MB (176018919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a6c62ff8157895ea7ef3e763fa3049b55594e2db3ce47f2ec757f68852cb1`  
		Last Modified: Fri, 18 Jun 2021 01:30:43 GMT  
		Size: 193.0 B  
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
$ docker pull ros@sha256:e1833adae51a31b60aca5b022dc72bba5e340d1a0bb93508f8261ba3f8362e6f
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
$ docker pull ros@sha256:cd2c29e97c22320da2aa6374649bee98a2cf5c52c32c0b7332e9c57da8b081ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385870031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6670bbcb18a0748c3e79f0e57e0b5a2bfc3ef4df56372ff9415f4ed34335362d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
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
$ docker pull ros@sha256:579a16c59836a20359c8404e4d3737fd70dde994e7904b2f1f6d0d13fd556c7e
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
$ docker pull ros@sha256:8bcb38422abde744ef1b47b41bbc421b1178c2ac3c9dd93b2a5f548ca72c3ffc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645746558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf81c41e9540d68b6f121d89fd22ef56b28f141e91196ff8faf4593f093ec192`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:38:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493c53114df8cfc9da74ef4264c753e21c1d1e595a13c1fa232d10586e9b4e82`  
		Last Modified: Fri, 18 Jun 2021 00:51:19 GMT  
		Size: 259.9 MB (259876527 bytes)  
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
$ docker pull ros@sha256:579a16c59836a20359c8404e4d3737fd70dde994e7904b2f1f6d0d13fd556c7e
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
$ docker pull ros@sha256:8bcb38422abde744ef1b47b41bbc421b1178c2ac3c9dd93b2a5f548ca72c3ffc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645746558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf81c41e9540d68b6f121d89fd22ef56b28f141e91196ff8faf4593f093ec192`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:38:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493c53114df8cfc9da74ef4264c753e21c1d1e595a13c1fa232d10586e9b4e82`  
		Last Modified: Fri, 18 Jun 2021 00:51:19 GMT  
		Size: 259.9 MB (259876527 bytes)  
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
$ docker pull ros@sha256:a77108ebd8e4b857da8ab441cae01a393dc9a3240f789d87338984e563f70174
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
$ docker pull ros@sha256:098efa72f6465e510d1cba1ed57579cc27835e2c234b9b1c63e65d08bc828ffd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395989359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d1dfe82351570470634cbef6d767d557590f4eec4ec744a3cf4cb66b330eeb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f842f4b28e2f0b0c088ea2bf3b105410a725bcfa21ed9bd0dd0011d7ee9f26ed`  
		Last Modified: Fri, 18 Jun 2021 00:50:09 GMT  
		Size: 10.1 MB (10119328 bytes)  
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
$ docker pull ros@sha256:a77108ebd8e4b857da8ab441cae01a393dc9a3240f789d87338984e563f70174
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
$ docker pull ros@sha256:098efa72f6465e510d1cba1ed57579cc27835e2c234b9b1c63e65d08bc828ffd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395989359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d1dfe82351570470634cbef6d767d557590f4eec4ec744a3cf4cb66b330eeb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f842f4b28e2f0b0c088ea2bf3b105410a725bcfa21ed9bd0dd0011d7ee9f26ed`  
		Last Modified: Fri, 18 Jun 2021 00:50:09 GMT  
		Size: 10.1 MB (10119328 bytes)  
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
$ docker pull ros@sha256:e1833adae51a31b60aca5b022dc72bba5e340d1a0bb93508f8261ba3f8362e6f
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
$ docker pull ros@sha256:cd2c29e97c22320da2aa6374649bee98a2cf5c52c32c0b7332e9c57da8b081ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385870031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6670bbcb18a0748c3e79f0e57e0b5a2bfc3ef4df56372ff9415f4ed34335362d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
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
$ docker pull ros@sha256:e1833adae51a31b60aca5b022dc72bba5e340d1a0bb93508f8261ba3f8362e6f
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
$ docker pull ros@sha256:cd2c29e97c22320da2aa6374649bee98a2cf5c52c32c0b7332e9c57da8b081ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385870031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6670bbcb18a0748c3e79f0e57e0b5a2bfc3ef4df56372ff9415f4ed34335362d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:36:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:36:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4290f747f0c4b4779b77f906be438c01282ea823564de8e051b6b5a32ed386`  
		Last Modified: Fri, 18 Jun 2021 00:49:45 GMT  
		Size: 54.7 MB (54694723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5ab3a0a26bfc2ecfa7750ec4eebb380f2bd507b32cc65716827f5d210b004`  
		Last Modified: Fri, 18 Jun 2021 00:49:32 GMT  
		Size: 267.6 KB (267557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac9b5a1ce10a0beb6ce33cea9517151a02abc67edcf7e9af2a4c292680533f`  
		Last Modified: Fri, 18 Jun 2021 00:49:49 GMT  
		Size: 64.7 MB (64743598 bytes)  
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
$ docker pull ros@sha256:a013f6031ea20184fa37669122470a6812e4e33fc871844a9671516b622d7eb7
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
$ docker pull ros@sha256:b8067b71e851eefe5dd43a7e6c32a8cc658ce18121a9d87d3a0693f7cf500ad5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266164153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fbe77d16723a1e9dd491a32ca4fe9d57c2645b7c966d6c0d36ce7790f5d4b73`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
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
$ docker pull ros@sha256:a013f6031ea20184fa37669122470a6812e4e33fc871844a9671516b622d7eb7
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
$ docker pull ros@sha256:b8067b71e851eefe5dd43a7e6c32a8cc658ce18121a9d87d3a0693f7cf500ad5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266164153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fbe77d16723a1e9dd491a32ca4fe9d57c2645b7c966d6c0d36ce7790f5d4b73`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:34:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:34:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:34:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:34:13 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:34:14 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:35:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:35:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e753b3b845373718d43d9bfa7e02513de354487e63eb5e48f7474a3d86f17405`  
		Last Modified: Fri, 18 Jun 2021 00:48:33 GMT  
		Size: 841.4 KB (841427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630d9b6692ef7c2820831e24519c3fbd127e5a81df87b4e92c244e3e76a0422`  
		Last Modified: Fri, 18 Jun 2021 00:48:31 GMT  
		Size: 4.1 MB (4085696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23cb6735c41513adec591f7e9e1e9e9cf2001a353cd5dc57a9477631748580`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e5f0587b277683f9470844328daee7603ad18c97c44579c714f5932ec1d4`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0956415e9e08d2620a690b9d752ff93361c150980530b52be5ac7cec77d547`  
		Last Modified: Fri, 18 Jun 2021 00:49:17 GMT  
		Size: 238.9 MB (238937014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc732f4453e348b5c26e63b4d49383bc6728abf935ba918480903cb1f37c35`  
		Last Modified: Fri, 18 Jun 2021 00:48:30 GMT  
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
$ docker pull ros@sha256:84f5968e3e142bf7b0d619ba67dc8e228898743ef3fd329d74be041226922594
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
$ docker pull ros@sha256:cbe95a64cfdaf927723119c35a44bc6e74458fb469f0dda63bb72dd3b886657b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283715127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c62e431459f3305175a89b0443a3b7f0fc76c8c11f930ccb8f4d20e453d2a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
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
$ docker pull ros@sha256:4805bc0c80e54e45a96c92eb281364439eb70ee51981465f1052c4a7ef00f9c0
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
$ docker pull ros@sha256:356abc77272b978828e7e1d9245247480e5412126c5ba99633b0aaa4270a421a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.3 MB (727286293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:173c7d8194149adbe9587fdae55c961c7070008f74fe72993bc5639851179e7e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:43:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5b383e2323174249cb8d972c0690b211c0fd883e821b2c125b4fca2289870e`  
		Last Modified: Fri, 18 Jun 2021 00:54:52 GMT  
		Size: 443.6 MB (443571166 bytes)  
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
$ docker pull ros@sha256:01490b742bf19bfa1123857eeaa53c5f8a432df5ca24db281526f35a838dd203
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:2866d5a9fd9a5f6100f24c6445ca31d7c67a791a1d1de78e49ea311c624f9881
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.0 MB (968027873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92b05b8c11d0c1b4491b4717215140ddc602822b27a45f1c08fbad43c9a6731`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:14:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:05:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Jun 2021 19:05:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Jun 2021 19:06:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:06:38 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:06:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:06:38 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:07:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:07:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:07:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a04ce26341db0d6591d2793ca267552485c51f4cbb273019ac821d671266ce`  
		Last Modified: Wed, 12 May 2021 17:24:25 GMT  
		Size: 10.9 MB (10891745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f874a1d96f3564e1336fb9600729be2ea22b555e7af860074cfac35ef5aca5a4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c733261a68b07a3b86e48d99685861b97f39fa9c98eb8faa30f5794651d1736d`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271be76f2de712a4f3df979ae1d086ffd0f695f5786c1914807e6f68c00bf367`  
		Last Modified: Wed, 02 Jun 2021 19:42:16 GMT  
		Size: 239.1 MB (239077729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa12225bfbe392ebc8cd18c1353c6ff079a250c0c1077d87f1466cfbd29234d4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6be44022cfad412873932550fcb4c91fe1a2a38a00a3a6ce5dc2f26cb787ef2`  
		Last Modified: Wed, 02 Jun 2021 19:42:38 GMT  
		Size: 86.6 MB (86566951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f606a538348e9f7f068265e12126380e56c095c967e463d0f1eaf77176823b9d`  
		Last Modified: Wed, 02 Jun 2021 19:42:24 GMT  
		Size: 299.6 KB (299563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b093daee989ce1c0f63e8151bbb0c5cd4b6876a277b3be6867b2e766d1e7985`  
		Last Modified: Wed, 02 Jun 2021 19:42:37 GMT  
		Size: 76.0 MB (75975246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435c89077a0df30ca6ec5a5b09388704cb368ee693473db9b2c967a969c77435`  
		Last Modified: Wed, 02 Jun 2021 19:44:33 GMT  
		Size: 504.8 MB (504780986 bytes)  
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
$ docker pull ros@sha256:4805bc0c80e54e45a96c92eb281364439eb70ee51981465f1052c4a7ef00f9c0
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
$ docker pull ros@sha256:356abc77272b978828e7e1d9245247480e5412126c5ba99633b0aaa4270a421a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.3 MB (727286293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:173c7d8194149adbe9587fdae55c961c7070008f74fe72993bc5639851179e7e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:43:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5b383e2323174249cb8d972c0690b211c0fd883e821b2c125b4fca2289870e`  
		Last Modified: Fri, 18 Jun 2021 00:54:52 GMT  
		Size: 443.6 MB (443571166 bytes)  
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
$ docker pull ros@sha256:da595a375f3dde1e04e3bfd55ad9acadaf272f97dfb49d8cfcb6857c28e8d33d
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
$ docker pull ros@sha256:f21b80eab15cb2e10f4911457fe7fba8b950f32e25c96887335238e6a8814255
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297674013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251efa79ee5cc97c24e7e8726f58151cc4ad2561ba09fefd0ea14bd4af5c69b9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:41:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb9c530dd9055920b4042e65c0b74d26c04f978e22b538e24b060b242626f`  
		Last Modified: Fri, 18 Jun 2021 00:53:06 GMT  
		Size: 14.0 MB (13958886 bytes)  
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
$ docker pull ros@sha256:ee14ce3b85619606e2812577e4a33afd92571b609ea355af7feeb47fdfe9a5d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:fe2b8f3c928c85d35277970898057f28837c470f7d1e5e8b6b06dcd38cc92226
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.5 MB (484467192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0966f35a10b7633880363d4d1f5a83bf4c81cf0d5a3cd2741c7c935687b9ef2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:14:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:05:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Jun 2021 19:05:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Jun 2021 19:06:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:06:38 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:06:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:06:38 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:07:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:07:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:07:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a04ce26341db0d6591d2793ca267552485c51f4cbb273019ac821d671266ce`  
		Last Modified: Wed, 12 May 2021 17:24:25 GMT  
		Size: 10.9 MB (10891745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f874a1d96f3564e1336fb9600729be2ea22b555e7af860074cfac35ef5aca5a4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c733261a68b07a3b86e48d99685861b97f39fa9c98eb8faa30f5794651d1736d`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271be76f2de712a4f3df979ae1d086ffd0f695f5786c1914807e6f68c00bf367`  
		Last Modified: Wed, 02 Jun 2021 19:42:16 GMT  
		Size: 239.1 MB (239077729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa12225bfbe392ebc8cd18c1353c6ff079a250c0c1077d87f1466cfbd29234d4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6be44022cfad412873932550fcb4c91fe1a2a38a00a3a6ce5dc2f26cb787ef2`  
		Last Modified: Wed, 02 Jun 2021 19:42:38 GMT  
		Size: 86.6 MB (86566951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f606a538348e9f7f068265e12126380e56c095c967e463d0f1eaf77176823b9d`  
		Last Modified: Wed, 02 Jun 2021 19:42:24 GMT  
		Size: 299.6 KB (299563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b093daee989ce1c0f63e8151bbb0c5cd4b6876a277b3be6867b2e766d1e7985`  
		Last Modified: Wed, 02 Jun 2021 19:42:37 GMT  
		Size: 76.0 MB (75975246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d38fa876c09e82dace7eab4ba3c214a03349d7435cf7d64f9b793138f9e9b6`  
		Last Modified: Wed, 02 Jun 2021 19:42:50 GMT  
		Size: 21.2 MB (21220305 bytes)  
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
$ docker pull ros@sha256:da595a375f3dde1e04e3bfd55ad9acadaf272f97dfb49d8cfcb6857c28e8d33d
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
$ docker pull ros@sha256:f21b80eab15cb2e10f4911457fe7fba8b950f32e25c96887335238e6a8814255
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297674013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251efa79ee5cc97c24e7e8726f58151cc4ad2561ba09fefd0ea14bd4af5c69b9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:41:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb9c530dd9055920b4042e65c0b74d26c04f978e22b538e24b060b242626f`  
		Last Modified: Fri, 18 Jun 2021 00:53:06 GMT  
		Size: 14.0 MB (13958886 bytes)  
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
$ docker pull ros@sha256:84f5968e3e142bf7b0d619ba67dc8e228898743ef3fd329d74be041226922594
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
$ docker pull ros@sha256:cbe95a64cfdaf927723119c35a44bc6e74458fb469f0dda63bb72dd3b886657b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283715127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c62e431459f3305175a89b0443a3b7f0fc76c8c11f930ccb8f4d20e453d2a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
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
$ docker pull ros@sha256:56fcca35a4963959668b2ba9e139d35fade75a76d494319a322613df19970ad6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:f9e9ba74302375bb5538519ee2deb1395ebe4e830313a417c3488cc18be46809
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463246887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdc2f6ac11d64fddb448ed58a0946459532a22ec3dc99f1ecfa0037074c628`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:14:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:05:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Jun 2021 19:05:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Jun 2021 19:06:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:06:38 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:06:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:06:38 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:07:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:07:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:07:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a04ce26341db0d6591d2793ca267552485c51f4cbb273019ac821d671266ce`  
		Last Modified: Wed, 12 May 2021 17:24:25 GMT  
		Size: 10.9 MB (10891745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f874a1d96f3564e1336fb9600729be2ea22b555e7af860074cfac35ef5aca5a4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c733261a68b07a3b86e48d99685861b97f39fa9c98eb8faa30f5794651d1736d`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271be76f2de712a4f3df979ae1d086ffd0f695f5786c1914807e6f68c00bf367`  
		Last Modified: Wed, 02 Jun 2021 19:42:16 GMT  
		Size: 239.1 MB (239077729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa12225bfbe392ebc8cd18c1353c6ff079a250c0c1077d87f1466cfbd29234d4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6be44022cfad412873932550fcb4c91fe1a2a38a00a3a6ce5dc2f26cb787ef2`  
		Last Modified: Wed, 02 Jun 2021 19:42:38 GMT  
		Size: 86.6 MB (86566951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f606a538348e9f7f068265e12126380e56c095c967e463d0f1eaf77176823b9d`  
		Last Modified: Wed, 02 Jun 2021 19:42:24 GMT  
		Size: 299.6 KB (299563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b093daee989ce1c0f63e8151bbb0c5cd4b6876a277b3be6867b2e766d1e7985`  
		Last Modified: Wed, 02 Jun 2021 19:42:37 GMT  
		Size: 76.0 MB (75975246 bytes)  
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
$ docker pull ros@sha256:84f5968e3e142bf7b0d619ba67dc8e228898743ef3fd329d74be041226922594
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
$ docker pull ros@sha256:cbe95a64cfdaf927723119c35a44bc6e74458fb469f0dda63bb72dd3b886657b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283715127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c62e431459f3305175a89b0443a3b7f0fc76c8c11f930ccb8f4d20e453d2a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbbe51271308fe6a1af1a169182b0f15582f368c872736775e764109f238983`  
		Last Modified: Fri, 18 Jun 2021 00:52:37 GMT  
		Size: 35.8 MB (35832534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835fe755c71537f5323873f30c148f7f77b4e38fb3feda80d127848da6110d0`  
		Last Modified: Fri, 18 Jun 2021 00:52:30 GMT  
		Size: 307.2 KB (307174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c08ad57952ad399129ef6732755ffe72648326f6eb85c67957c08133b5a09`  
		Last Modified: Fri, 18 Jun 2021 00:52:44 GMT  
		Size: 60.5 MB (60481071 bytes)  
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
$ docker pull ros@sha256:19eeb2e978c2e6f00f0fd10427ff6de6efac08f0d10fdf80fbeb297e285cad8d
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
$ docker pull ros@sha256:0126dbfd7c3dc1d7cd91e7bdade2b2ec0e6b378dea1ba41198efc4bd4b67e594
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187094348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b049fb02175a4972cc7fef1ac4ad7888fc312b21aa871e0639c8aa99c6cefa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
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
$ docker pull ros@sha256:5e60ff8fbbd35edff105c02fb6259b85c62af0da8d3593ec5f015726af9151b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:1d3c9e0a79a45639c4a19679174c58ee7cca3f2baae2ebdc72aaf55602b8be3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300405127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0abbf54342c91585a7e43b4d229e64ac8b8987f1d48570a24b62dd2c1979a97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:14:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:05:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Jun 2021 19:05:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Jun 2021 19:06:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:06:38 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:06:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:06:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a04ce26341db0d6591d2793ca267552485c51f4cbb273019ac821d671266ce`  
		Last Modified: Wed, 12 May 2021 17:24:25 GMT  
		Size: 10.9 MB (10891745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f874a1d96f3564e1336fb9600729be2ea22b555e7af860074cfac35ef5aca5a4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c733261a68b07a3b86e48d99685861b97f39fa9c98eb8faa30f5794651d1736d`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271be76f2de712a4f3df979ae1d086ffd0f695f5786c1914807e6f68c00bf367`  
		Last Modified: Wed, 02 Jun 2021 19:42:16 GMT  
		Size: 239.1 MB (239077729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa12225bfbe392ebc8cd18c1353c6ff079a250c0c1077d87f1466cfbd29234d4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
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
$ docker pull ros@sha256:19eeb2e978c2e6f00f0fd10427ff6de6efac08f0d10fdf80fbeb297e285cad8d
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
$ docker pull ros@sha256:0126dbfd7c3dc1d7cd91e7bdade2b2ec0e6b378dea1ba41198efc4bd4b67e594
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187094348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b049fb02175a4972cc7fef1ac4ad7888fc312b21aa871e0639c8aa99c6cefa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:39:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 00:39:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 00:39:26 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 00:40:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 00:40:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 00:40:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8cede0e2e2dd5d208ef924463c999e69cb6fc1ba2307638552691d952b69fc`  
		Last Modified: Fri, 18 Jun 2021 00:51:37 GMT  
		Size: 1.2 MB (1183539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270aed8a77df54e18c79b0a229b46987065bb0ea02f33648a733798958dd0f6b`  
		Last Modified: Fri, 18 Jun 2021 00:51:35 GMT  
		Size: 4.7 MB (4676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a5b1478dbbb8fb8e8bfd33a08ff80bab33be91503bb30a54b726281c8a9`  
		Last Modified: Fri, 18 Jun 2021 00:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3303d4a12b07ea1903b5cc79b486342c231dd7dd39a9453e932141e7f1f1`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aff3d1855dc9605e8ff882bf0ef6f3a2070675e76f4ffc0e3b2232bde2182`  
		Last Modified: Fri, 18 Jun 2021 00:52:16 GMT  
		Size: 157.2 MB (157180161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11687330ead2d1d115616c6d694c08854445c59caa4b0772837df8c2e0a87f2`  
		Last Modified: Fri, 18 Jun 2021 00:51:34 GMT  
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
