<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:humble`](#roshumble)
-	[`ros:humble-perception`](#roshumble-perception)
-	[`ros:humble-perception-jammy`](#roshumble-perception-jammy)
-	[`ros:humble-ros-base`](#roshumble-ros-base)
-	[`ros:humble-ros-base-jammy`](#roshumble-ros-base-jammy)
-	[`ros:humble-ros-core`](#roshumble-ros-core)
-	[`ros:humble-ros-core-jammy`](#roshumble-ros-core-jammy)
-	[`ros:iron`](#rosiron)
-	[`ros:iron-perception`](#rosiron-perception)
-	[`ros:iron-perception-jammy`](#rosiron-perception-jammy)
-	[`ros:iron-ros-base`](#rosiron-ros-base)
-	[`ros:iron-ros-base-jammy`](#rosiron-ros-base-jammy)
-	[`ros:iron-ros-core`](#rosiron-ros-core)
-	[`ros:iron-ros-core-jammy`](#rosiron-ros-core-jammy)
-	[`ros:latest`](#roslatest)
-	[`ros:noetic`](#rosnoetic)
-	[`ros:noetic-perception`](#rosnoetic-perception)
-	[`ros:noetic-perception-focal`](#rosnoetic-perception-focal)
-	[`ros:noetic-robot`](#rosnoetic-robot)
-	[`ros:noetic-robot-focal`](#rosnoetic-robot-focal)
-	[`ros:noetic-ros-base`](#rosnoetic-ros-base)
-	[`ros:noetic-ros-base-focal`](#rosnoetic-ros-base-focal)
-	[`ros:noetic-ros-core`](#rosnoetic-ros-core)
-	[`ros:noetic-ros-core-focal`](#rosnoetic-ros-core-focal)
-	[`ros:rolling`](#rosrolling)
-	[`ros:rolling-perception`](#rosrolling-perception)
-	[`ros:rolling-perception-jammy`](#rosrolling-perception-jammy)
-	[`ros:rolling-ros-base`](#rosrolling-ros-base)
-	[`ros:rolling-ros-base-jammy`](#rosrolling-ros-base-jammy)
-	[`ros:rolling-ros-core`](#rosrolling-ros-core)
-	[`ros:rolling-ros-core-jammy`](#rosrolling-ros-core-jammy)

## `ros:humble`

```console
$ docker pull ros@sha256:34625aa8e7c2a90e39a7ad83cefe59281ac4bc174c7236b63122131d2b4b5fa3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:54d8ab351fd3fda6d646759df9f6741e6ccc3a9a75c9645e3616d830bf2a13ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263402877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc6355d9492ebd485370791a6aee424c17bf5e92ecccd178e058c50e2d3577`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7cf7c4046fa3d89d06e305fc81f2b45c6acbd04568c50f63955574b8b5a0b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (256049477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b25c0705a1b8bf5a82f9e10e143b13c3f21c8ba7e3319ff14a8ff637185bea8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:39828be6397f30e54b0629ec7df3d526f49d4af4276245afbec6ba265fb4c146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:5e5ea6fd504d3d0a45bd8c464e0d9da7c113d318d6ee9a346c8a1cd4fba7b8c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **953.6 MB (953584554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc9075856b7daa752a9aff6d139115ff9db78fe2cf98222c71740a1003e2697`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:43:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7bd313849f09cf70f1a2108141db6f7610dc479829316180863437ffc52a1`  
		Last Modified: Sat, 02 Sep 2023 01:52:52 GMT  
		Size: 690.2 MB (690181677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1012f29357f78f9bb00ce55bfc95072973d6ae73627674b5ef4837114001aa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **914.1 MB (914088422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2193a560c90e7968ca85465a319d367d990e8026e8a668ee951ee34c2da0fc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8590d691e0846807c4802d8a4a74d60b6d0600c0a2d1cc6da88d0e6899e06d8`  
		Last Modified: Sat, 02 Sep 2023 00:45:14 GMT  
		Size: 658.0 MB (658038945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:39828be6397f30e54b0629ec7df3d526f49d4af4276245afbec6ba265fb4c146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:5e5ea6fd504d3d0a45bd8c464e0d9da7c113d318d6ee9a346c8a1cd4fba7b8c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **953.6 MB (953584554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc9075856b7daa752a9aff6d139115ff9db78fe2cf98222c71740a1003e2697`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:43:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7bd313849f09cf70f1a2108141db6f7610dc479829316180863437ffc52a1`  
		Last Modified: Sat, 02 Sep 2023 01:52:52 GMT  
		Size: 690.2 MB (690181677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1012f29357f78f9bb00ce55bfc95072973d6ae73627674b5ef4837114001aa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **914.1 MB (914088422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2193a560c90e7968ca85465a319d367d990e8026e8a668ee951ee34c2da0fc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8590d691e0846807c4802d8a4a74d60b6d0600c0a2d1cc6da88d0e6899e06d8`  
		Last Modified: Sat, 02 Sep 2023 00:45:14 GMT  
		Size: 658.0 MB (658038945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:34625aa8e7c2a90e39a7ad83cefe59281ac4bc174c7236b63122131d2b4b5fa3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:54d8ab351fd3fda6d646759df9f6741e6ccc3a9a75c9645e3616d830bf2a13ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263402877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc6355d9492ebd485370791a6aee424c17bf5e92ecccd178e058c50e2d3577`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7cf7c4046fa3d89d06e305fc81f2b45c6acbd04568c50f63955574b8b5a0b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (256049477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b25c0705a1b8bf5a82f9e10e143b13c3f21c8ba7e3319ff14a8ff637185bea8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:34625aa8e7c2a90e39a7ad83cefe59281ac4bc174c7236b63122131d2b4b5fa3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:54d8ab351fd3fda6d646759df9f6741e6ccc3a9a75c9645e3616d830bf2a13ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263402877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc6355d9492ebd485370791a6aee424c17bf5e92ecccd178e058c50e2d3577`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7cf7c4046fa3d89d06e305fc81f2b45c6acbd04568c50f63955574b8b5a0b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (256049477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b25c0705a1b8bf5a82f9e10e143b13c3f21c8ba7e3319ff14a8ff637185bea8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:1e5e7aee07e8bdca93b61f92865e362ceffce611367fd2b9e7d8fd1b169acf48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:e9f7271f5f26b0b507eff63793598e34e1e25f4049052ac6e747b1176bb3a9bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141876968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92bd81cb6beb0143e6eff5dba7d115f1fd727bff7221ba2da46354d427404594`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:28d4b8a5ca47a67451c7508dadf61f5d60a7047bfda2b83e879fb8d59689d877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137537553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c18648c5967b2fb8817b85a27460153ad98242dc0fab345c1c90ad4cd9a20a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:1e5e7aee07e8bdca93b61f92865e362ceffce611367fd2b9e7d8fd1b169acf48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e9f7271f5f26b0b507eff63793598e34e1e25f4049052ac6e747b1176bb3a9bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141876968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92bd81cb6beb0143e6eff5dba7d115f1fd727bff7221ba2da46354d427404594`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:28d4b8a5ca47a67451c7508dadf61f5d60a7047bfda2b83e879fb8d59689d877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137537553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c18648c5967b2fb8817b85a27460153ad98242dc0fab345c1c90ad4cd9a20a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron`

```console
$ docker pull ros@sha256:6df9b084cb7e918455df628126b2b647d2ad2e4b0e979fb8fbc525a610573bbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron` - linux; amd64

```console
$ docker pull ros@sha256:19f9d8868c1e347029475a838c9c765286c141e6a673b2f31ed6e5c7045af5b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268812427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:566511b861bd52dde141dae0914d63a5eb14850a6f4c0ff174407213eaa27f10`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:44:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:44:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32443c3ac64e04b22d6797ee761ea18ca5c4749eb5a2dcae8266d2684aaed2ce`  
		Last Modified: Sat, 02 Sep 2023 01:53:39 GMT  
		Size: 85.2 MB (85155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ac734be63315b3b63b781efcbaa8722df32b756426076cd7162d668e0c33b`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 301.8 KB (301785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443793671c0c8e8e8c531e037c8fee594f63f987915e16e3453604520da34b50`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 2.4 KB (2429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571dcb4ca7607bd065dfecf00e9fc01451d08d3c1625e0088df997582acb24c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:32 GMT  
		Size: 23.7 MB (23725382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31a5be63ab3b2fe0edd2aa2a6cc114a8d681c7b43bace413d0d67dd215dc958a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.3 MB (261313267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb5b932dd24d525cfc727ed1de564380748feed2f728000e8a3c38b41087348`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:36:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:37:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcb57bc4c7d7e86f5a699347526dd36d6d6a796ca281a1c43190a17b675f70d`  
		Last Modified: Sat, 02 Sep 2023 00:46:00 GMT  
		Size: 82.8 MB (82840292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472afd96ac321a5e6cadf1a1f9d0468065b38db7177e38ee01ef8f5caa1a426`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 301.8 KB (301784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792c71e1cd7464d234a82b207e6d65c1d368e11b7d519a91a05eed7c028cb33d`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 2.4 KB (2436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3335d0568506900d516401d3bb154f04e931bb4304218a71377ef3c4a8286c`  
		Last Modified: Sat, 02 Sep 2023 00:45:56 GMT  
		Size: 23.1 MB (23115925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception`

```console
$ docker pull ros@sha256:c06629c4d15658f8e2a666fc8983ec3e4c0d8c075cfaefe50291efa425334491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception` - linux; amd64

```console
$ docker pull ros@sha256:2b2f9d66370cfda7a91d8e0e6ee55af2b27ab2487382ac63edd19d477bc0b5e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.7 MB (959704912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46f035788f2871ea56661de3c07768a00b3aecd34403a57401e703287e75bdf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:44:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:44:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32443c3ac64e04b22d6797ee761ea18ca5c4749eb5a2dcae8266d2684aaed2ce`  
		Last Modified: Sat, 02 Sep 2023 01:53:39 GMT  
		Size: 85.2 MB (85155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ac734be63315b3b63b781efcbaa8722df32b756426076cd7162d668e0c33b`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 301.8 KB (301785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443793671c0c8e8e8c531e037c8fee594f63f987915e16e3453604520da34b50`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 2.4 KB (2429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571dcb4ca7607bd065dfecf00e9fc01451d08d3c1625e0088df997582acb24c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:32 GMT  
		Size: 23.7 MB (23725382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b027d64a215a4fe959ba8f55d39ff5b6fdf732f0bca77b1d446e0ddb154d54d9`  
		Last Modified: Sat, 02 Sep 2023 01:55:17 GMT  
		Size: 690.9 MB (690892485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:96868053101d2313b0464f09c9e478ffd49487b41f4c2ac007dafcee702ded5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.0 MB (919973844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d3c4ae393fe7c8927bd220b4d15dc36e6b9a0baee35080d72f2487f7ccdf00`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:36:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:37:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcb57bc4c7d7e86f5a699347526dd36d6d6a796ca281a1c43190a17b675f70d`  
		Last Modified: Sat, 02 Sep 2023 00:46:00 GMT  
		Size: 82.8 MB (82840292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472afd96ac321a5e6cadf1a1f9d0468065b38db7177e38ee01ef8f5caa1a426`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 301.8 KB (301784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792c71e1cd7464d234a82b207e6d65c1d368e11b7d519a91a05eed7c028cb33d`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 2.4 KB (2436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3335d0568506900d516401d3bb154f04e931bb4304218a71377ef3c4a8286c`  
		Last Modified: Sat, 02 Sep 2023 00:45:56 GMT  
		Size: 23.1 MB (23115925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2223c6ec49752449f5935b69b8908839a7f8afd293ea6e1b278961e66b9129`  
		Last Modified: Sat, 02 Sep 2023 00:47:28 GMT  
		Size: 658.7 MB (658660577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:c06629c4d15658f8e2a666fc8983ec3e4c0d8c075cfaefe50291efa425334491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:2b2f9d66370cfda7a91d8e0e6ee55af2b27ab2487382ac63edd19d477bc0b5e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.7 MB (959704912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46f035788f2871ea56661de3c07768a00b3aecd34403a57401e703287e75bdf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:44:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:44:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32443c3ac64e04b22d6797ee761ea18ca5c4749eb5a2dcae8266d2684aaed2ce`  
		Last Modified: Sat, 02 Sep 2023 01:53:39 GMT  
		Size: 85.2 MB (85155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ac734be63315b3b63b781efcbaa8722df32b756426076cd7162d668e0c33b`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 301.8 KB (301785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443793671c0c8e8e8c531e037c8fee594f63f987915e16e3453604520da34b50`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 2.4 KB (2429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571dcb4ca7607bd065dfecf00e9fc01451d08d3c1625e0088df997582acb24c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:32 GMT  
		Size: 23.7 MB (23725382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b027d64a215a4fe959ba8f55d39ff5b6fdf732f0bca77b1d446e0ddb154d54d9`  
		Last Modified: Sat, 02 Sep 2023 01:55:17 GMT  
		Size: 690.9 MB (690892485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:96868053101d2313b0464f09c9e478ffd49487b41f4c2ac007dafcee702ded5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.0 MB (919973844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d3c4ae393fe7c8927bd220b4d15dc36e6b9a0baee35080d72f2487f7ccdf00`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:36:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:37:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcb57bc4c7d7e86f5a699347526dd36d6d6a796ca281a1c43190a17b675f70d`  
		Last Modified: Sat, 02 Sep 2023 00:46:00 GMT  
		Size: 82.8 MB (82840292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472afd96ac321a5e6cadf1a1f9d0468065b38db7177e38ee01ef8f5caa1a426`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 301.8 KB (301784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792c71e1cd7464d234a82b207e6d65c1d368e11b7d519a91a05eed7c028cb33d`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 2.4 KB (2436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3335d0568506900d516401d3bb154f04e931bb4304218a71377ef3c4a8286c`  
		Last Modified: Sat, 02 Sep 2023 00:45:56 GMT  
		Size: 23.1 MB (23115925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2223c6ec49752449f5935b69b8908839a7f8afd293ea6e1b278961e66b9129`  
		Last Modified: Sat, 02 Sep 2023 00:47:28 GMT  
		Size: 658.7 MB (658660577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base`

```console
$ docker pull ros@sha256:6df9b084cb7e918455df628126b2b647d2ad2e4b0e979fb8fbc525a610573bbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:19f9d8868c1e347029475a838c9c765286c141e6a673b2f31ed6e5c7045af5b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268812427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:566511b861bd52dde141dae0914d63a5eb14850a6f4c0ff174407213eaa27f10`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:44:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:44:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32443c3ac64e04b22d6797ee761ea18ca5c4749eb5a2dcae8266d2684aaed2ce`  
		Last Modified: Sat, 02 Sep 2023 01:53:39 GMT  
		Size: 85.2 MB (85155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ac734be63315b3b63b781efcbaa8722df32b756426076cd7162d668e0c33b`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 301.8 KB (301785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443793671c0c8e8e8c531e037c8fee594f63f987915e16e3453604520da34b50`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 2.4 KB (2429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571dcb4ca7607bd065dfecf00e9fc01451d08d3c1625e0088df997582acb24c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:32 GMT  
		Size: 23.7 MB (23725382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31a5be63ab3b2fe0edd2aa2a6cc114a8d681c7b43bace413d0d67dd215dc958a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.3 MB (261313267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb5b932dd24d525cfc727ed1de564380748feed2f728000e8a3c38b41087348`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:36:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:37:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcb57bc4c7d7e86f5a699347526dd36d6d6a796ca281a1c43190a17b675f70d`  
		Last Modified: Sat, 02 Sep 2023 00:46:00 GMT  
		Size: 82.8 MB (82840292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472afd96ac321a5e6cadf1a1f9d0468065b38db7177e38ee01ef8f5caa1a426`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 301.8 KB (301784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792c71e1cd7464d234a82b207e6d65c1d368e11b7d519a91a05eed7c028cb33d`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 2.4 KB (2436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3335d0568506900d516401d3bb154f04e931bb4304218a71377ef3c4a8286c`  
		Last Modified: Sat, 02 Sep 2023 00:45:56 GMT  
		Size: 23.1 MB (23115925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base-jammy`

```console
$ docker pull ros@sha256:6df9b084cb7e918455df628126b2b647d2ad2e4b0e979fb8fbc525a610573bbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:19f9d8868c1e347029475a838c9c765286c141e6a673b2f31ed6e5c7045af5b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268812427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:566511b861bd52dde141dae0914d63a5eb14850a6f4c0ff174407213eaa27f10`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:44:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:44:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32443c3ac64e04b22d6797ee761ea18ca5c4749eb5a2dcae8266d2684aaed2ce`  
		Last Modified: Sat, 02 Sep 2023 01:53:39 GMT  
		Size: 85.2 MB (85155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ac734be63315b3b63b781efcbaa8722df32b756426076cd7162d668e0c33b`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 301.8 KB (301785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443793671c0c8e8e8c531e037c8fee594f63f987915e16e3453604520da34b50`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 2.4 KB (2429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571dcb4ca7607bd065dfecf00e9fc01451d08d3c1625e0088df997582acb24c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:32 GMT  
		Size: 23.7 MB (23725382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31a5be63ab3b2fe0edd2aa2a6cc114a8d681c7b43bace413d0d67dd215dc958a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.3 MB (261313267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb5b932dd24d525cfc727ed1de564380748feed2f728000e8a3c38b41087348`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:36:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:37:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcb57bc4c7d7e86f5a699347526dd36d6d6a796ca281a1c43190a17b675f70d`  
		Last Modified: Sat, 02 Sep 2023 00:46:00 GMT  
		Size: 82.8 MB (82840292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472afd96ac321a5e6cadf1a1f9d0468065b38db7177e38ee01ef8f5caa1a426`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 301.8 KB (301784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792c71e1cd7464d234a82b207e6d65c1d368e11b7d519a91a05eed7c028cb33d`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 2.4 KB (2436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3335d0568506900d516401d3bb154f04e931bb4304218a71377ef3c4a8286c`  
		Last Modified: Sat, 02 Sep 2023 00:45:56 GMT  
		Size: 23.1 MB (23115925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core`

```console
$ docker pull ros@sha256:9680869872488aba382ba4ff5bb2530ef1f4ff5bd4243d113b2b5ee17bfca9b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:b28d51bd701613450e789b79fe4b2af444e54c1d3541167f5f67dcc0f0f78ea5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159627394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5d3dd94fe64c40fe3ceee428a70a97107686e911e51f222b788bed269f14dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0a3869eba7dc623982abda52ac00c6541c4a7cf5b9409c03740dbf3f130412c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155052830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dbf73008eafcee1b18d9ad8fed6c4c9963a8d2a06c60873fc08435da411082`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core-jammy`

```console
$ docker pull ros@sha256:9680869872488aba382ba4ff5bb2530ef1f4ff5bd4243d113b2b5ee17bfca9b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:b28d51bd701613450e789b79fe4b2af444e54c1d3541167f5f67dcc0f0f78ea5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159627394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5d3dd94fe64c40fe3ceee428a70a97107686e911e51f222b788bed269f14dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0a3869eba7dc623982abda52ac00c6541c4a7cf5b9409c03740dbf3f130412c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155052830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dbf73008eafcee1b18d9ad8fed6c4c9963a8d2a06c60873fc08435da411082`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:34625aa8e7c2a90e39a7ad83cefe59281ac4bc174c7236b63122131d2b4b5fa3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:54d8ab351fd3fda6d646759df9f6741e6ccc3a9a75c9645e3616d830bf2a13ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263402877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc6355d9492ebd485370791a6aee424c17bf5e92ecccd178e058c50e2d3577`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7cf7c4046fa3d89d06e305fc81f2b45c6acbd04568c50f63955574b8b5a0b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (256049477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b25c0705a1b8bf5a82f9e10e143b13c3f21c8ba7e3319ff14a8ff637185bea8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:a0e673042e87fff930781030b2c4244043147c52ebacb58952751a4f315cee7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:650483554542d585af1f7c6fd09a4fb64d1492243f19010662e5434e1489a9d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343156918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2661096a96da02ad942658f95aacd228d2d94aaa5334a9cc005367b9b88752`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ed655ce2187b5915ce130f9ff76436bfe8e526576d42ff1c4dbe1cf6fe400251
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289207245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3119f354b09e51524fefdb9ef586d2dc773ab7124fc788a3667cc2bb9f1d6977`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:af745a514f22826555b963a1881e2dccd9c605adb40b1b806c3c8f341f1104ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322829356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1df96a9ed3cefbb4a8d610a2cddeff2a565833d4813d072eba7794e8537e156`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:6a65a71812b94811599d640ab2710a224520253f53b10ce69d444eded20c36f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:ae2d31efb881f34de3d03d52d5addf87ee8125d1f886bf15babb5a1282242e1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835209394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23606c67a6f8bb711cbadbca4920eae8cfa1f0820596be362c1728e5f1f4ab40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:30:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072cf6370b84c85da7ec392f4f550ee0e9e157b32afafab89c2d75a944cc33dd`  
		Last Modified: Thu, 17 Aug 2023 07:51:42 GMT  
		Size: 492.1 MB (492052476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:4568955fd8353599a114b9795af7e1051a4da0570b63224d25fbd7d4d83d90ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726217529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c0f7621af902447b54ab155d89fb2d502e68a59df7ef4ade4b9a7fe2cd5740`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc7fb7f28f7754b8ebdd93a3161899a78031a37f823386f15f9980eed132431`  
		Last Modified: Sat, 02 Sep 2023 00:11:35 GMT  
		Size: 437.0 MB (437010284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7eae4b6fc8ff5ef942d83dcc51945e0c990c916ca2d4752a9a6421e1417fbadd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785516952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:873edfa41699dd21bb3bdb186b60357ffbe0860cd42dd6ae2524d61469cae46f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:16:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f409290bb4b094d2c155c6fc2d027cb969bc2ef37077101bc931a340cd2313`  
		Last Modified: Wed, 16 Aug 2023 15:38:46 GMT  
		Size: 462.7 MB (462687596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:6a65a71812b94811599d640ab2710a224520253f53b10ce69d444eded20c36f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:ae2d31efb881f34de3d03d52d5addf87ee8125d1f886bf15babb5a1282242e1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835209394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23606c67a6f8bb711cbadbca4920eae8cfa1f0820596be362c1728e5f1f4ab40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:30:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072cf6370b84c85da7ec392f4f550ee0e9e157b32afafab89c2d75a944cc33dd`  
		Last Modified: Thu, 17 Aug 2023 07:51:42 GMT  
		Size: 492.1 MB (492052476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:4568955fd8353599a114b9795af7e1051a4da0570b63224d25fbd7d4d83d90ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726217529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c0f7621af902447b54ab155d89fb2d502e68a59df7ef4ade4b9a7fe2cd5740`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc7fb7f28f7754b8ebdd93a3161899a78031a37f823386f15f9980eed132431`  
		Last Modified: Sat, 02 Sep 2023 00:11:35 GMT  
		Size: 437.0 MB (437010284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7eae4b6fc8ff5ef942d83dcc51945e0c990c916ca2d4752a9a6421e1417fbadd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785516952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:873edfa41699dd21bb3bdb186b60357ffbe0860cd42dd6ae2524d61469cae46f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:16:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f409290bb4b094d2c155c6fc2d027cb969bc2ef37077101bc931a340cd2313`  
		Last Modified: Wed, 16 Aug 2023 15:38:46 GMT  
		Size: 462.7 MB (462687596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:46642c256eb9803035dfaf81be09796e188a24d5a89ecd123c18bc9a0e2ec2f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:26171861e9728cd5afc87ff920583f1da58207535c4fabbab64bcb1914d761d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359019674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27dc1d4306276c53aaf0e61662f2418be18eabe34ff5b4173a789eb77f9d05d2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f781912f3aa6add79d8d355f91f4f813ea41cb3588b44b0946845b83c495dc3`  
		Last Modified: Thu, 17 Aug 2023 07:50:27 GMT  
		Size: 15.9 MB (15862756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:1445d42b4679bab7b680d2c3f519fb77fe91389baf443213cb56a0383e8776be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303276297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14f598bbd48caa2508a2f957ed678eca19bc3394214feab23e6232e68c4b451`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604b84d2e9735235fefc2e28067e6d4578944fd340a49da75b644ea17932be89`  
		Last Modified: Sat, 02 Sep 2023 00:10:27 GMT  
		Size: 14.1 MB (14069052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:48d1881e37fcb8aabdfd93a2ab3aa832f7ca9d42797cbbdbd0ab2b4aac829f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338288463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6195bda8b1ee1a176e4fbbec8431d1c7cb9f28b870ba66f4696467d40eb15340`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:08:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32ed50b6caa08d0a39dad2e4595bc889af7a598fcb07785b3eb4b8dc27869f`  
		Last Modified: Wed, 16 Aug 2023 15:37:38 GMT  
		Size: 15.5 MB (15459107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:46642c256eb9803035dfaf81be09796e188a24d5a89ecd123c18bc9a0e2ec2f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:26171861e9728cd5afc87ff920583f1da58207535c4fabbab64bcb1914d761d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359019674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27dc1d4306276c53aaf0e61662f2418be18eabe34ff5b4173a789eb77f9d05d2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f781912f3aa6add79d8d355f91f4f813ea41cb3588b44b0946845b83c495dc3`  
		Last Modified: Thu, 17 Aug 2023 07:50:27 GMT  
		Size: 15.9 MB (15862756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:1445d42b4679bab7b680d2c3f519fb77fe91389baf443213cb56a0383e8776be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303276297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14f598bbd48caa2508a2f957ed678eca19bc3394214feab23e6232e68c4b451`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604b84d2e9735235fefc2e28067e6d4578944fd340a49da75b644ea17932be89`  
		Last Modified: Sat, 02 Sep 2023 00:10:27 GMT  
		Size: 14.1 MB (14069052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:48d1881e37fcb8aabdfd93a2ab3aa832f7ca9d42797cbbdbd0ab2b4aac829f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338288463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6195bda8b1ee1a176e4fbbec8431d1c7cb9f28b870ba66f4696467d40eb15340`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:08:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32ed50b6caa08d0a39dad2e4595bc889af7a598fcb07785b3eb4b8dc27869f`  
		Last Modified: Wed, 16 Aug 2023 15:37:38 GMT  
		Size: 15.5 MB (15459107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:a0e673042e87fff930781030b2c4244043147c52ebacb58952751a4f315cee7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:650483554542d585af1f7c6fd09a4fb64d1492243f19010662e5434e1489a9d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343156918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2661096a96da02ad942658f95aacd228d2d94aaa5334a9cc005367b9b88752`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:ed655ce2187b5915ce130f9ff76436bfe8e526576d42ff1c4dbe1cf6fe400251
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289207245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3119f354b09e51524fefdb9ef586d2dc773ab7124fc788a3667cc2bb9f1d6977`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:af745a514f22826555b963a1881e2dccd9c605adb40b1b806c3c8f341f1104ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322829356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1df96a9ed3cefbb4a8d610a2cddeff2a565833d4813d072eba7794e8537e156`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:a0e673042e87fff930781030b2c4244043147c52ebacb58952751a4f315cee7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:650483554542d585af1f7c6fd09a4fb64d1492243f19010662e5434e1489a9d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343156918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2661096a96da02ad942658f95aacd228d2d94aaa5334a9cc005367b9b88752`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 07:24:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:24:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Aug 2023 07:25:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71044449a9df53317087cbf1480ae89d0864ed6c767b63f246f2a112cb697023`  
		Last Modified: Thu, 17 Aug 2023 07:50:07 GMT  
		Size: 50.9 MB (50940393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57c22656c0736ccbe5b757eeada9768c4061541ea8fced3debcc9d8e5186c3`  
		Last Modified: Thu, 17 Aug 2023 07:49:59 GMT  
		Size: 305.0 KB (305044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01916643bc85febc6c44576e168005fd7892f275d1a187528964c1a062bb36a`  
		Last Modified: Thu, 17 Aug 2023 07:50:10 GMT  
		Size: 79.6 MB (79614040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:ed655ce2187b5915ce130f9ff76436bfe8e526576d42ff1c4dbe1cf6fe400251
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289207245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3119f354b09e51524fefdb9ef586d2dc773ab7124fc788a3667cc2bb9f1d6977`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
# Fri, 01 Sep 2023 23:58:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:58:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:00:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f373e58003e6feec6779ea8963a18f8eef83cccb8692c45fd23e06aae9f2f85d`  
		Last Modified: Sat, 02 Sep 2023 00:10:11 GMT  
		Size: 40.5 MB (40504622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc3dcf367a02a485217499628d1fe2293b012c45f33b9634ff07e99f3c951`  
		Last Modified: Sat, 02 Sep 2023 00:10:05 GMT  
		Size: 306.5 KB (306514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28dc5824eafe60b35ff17147f8e22ec58457fe80c7d5c6b328cd4b4b959b9c4`  
		Last Modified: Sat, 02 Sep 2023 00:10:14 GMT  
		Size: 60.5 MB (60500243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:af745a514f22826555b963a1881e2dccd9c605adb40b1b806c3c8f341f1104ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322829356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1df96a9ed3cefbb4a8d610a2cddeff2a565833d4813d072eba7794e8537e156`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:06:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:06:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Aug 2023 15:07:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5211a2259bc1478e29b4690b53e5d12a125494f0f9a72cbfeeecbd7ec25e03b`  
		Last Modified: Wed, 16 Aug 2023 15:37:21 GMT  
		Size: 45.2 MB (45205544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7378851344c17811607f8ba6396d28e3461695a329ed8350d4cf455cd5c084`  
		Last Modified: Wed, 16 Aug 2023 15:37:15 GMT  
		Size: 305.0 KB (305028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3c47600689adaa3ce673c9171bc7b632548702a735bc4ed1b99f651d96fcb`  
		Last Modified: Wed, 16 Aug 2023 15:37:24 GMT  
		Size: 72.0 MB (71972732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:cc4ee72d153917d7891ea0271061c330ee1d3783ff5806b3f92bbbd2949e6a1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:4567c93b88b61349305b4d46a5ab1db18e13e687f8cf7c044516b0a1317d0b1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212297441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48feda2e6ad6031588e90d77629741370feaca36cd10958f6a8aefd3613c704f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3cecfb2ee2a353ee64507fc5771dde4438c61ed4f1daa304a20eb226b603d05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187895866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147bf0c6afbb97b0f5b7a60615f72c17f11b3f62601b2375433a3eff22aaa36f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f2439b922cac680e8c6cefcb54a18fa0c06efa19f290e0c7106c287944c9b1b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205346052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f02c719ef94496b7e6b92b6f5e381407904a4ca59c2e0b0fd8efc218cea02ae`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:cc4ee72d153917d7891ea0271061c330ee1d3783ff5806b3f92bbbd2949e6a1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:4567c93b88b61349305b4d46a5ab1db18e13e687f8cf7c044516b0a1317d0b1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212297441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48feda2e6ad6031588e90d77629741370feaca36cd10958f6a8aefd3613c704f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:21:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Aug 2023 07:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Aug 2023 07:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 07:21:52 GMT
ENV ROS_DISTRO=noetic
# Thu, 17 Aug 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:23:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 17 Aug 2023 07:23:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Aug 2023 07:23:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b915067b2cb577e1158572cfb9bb4edba91b52a0f5821152a8a4e2518dd702c`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 5.6 MB (5553744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd0b38cb0829def318257a357f2d9773c0c0f443432fe0ab8f0e28f8454a13`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b104afafaf102a6ecd5bc760e922c728c4ab27320895943844d8f53c908a025`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f437788a75a65f6ba1decf914b73eaf4b4712c46e542abaf9d51e92f1e6c32`  
		Last Modified: Thu, 17 Aug 2023 07:49:46 GMT  
		Size: 177.0 MB (176961988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8de474ce644ddf64e37acf737479db384d569592e927234ba9775cbf3c044`  
		Last Modified: Thu, 17 Aug 2023 07:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3cecfb2ee2a353ee64507fc5771dde4438c61ed4f1daa304a20eb226b603d05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187895866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147bf0c6afbb97b0f5b7a60615f72c17f11b3f62601b2375433a3eff22aaa36f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:07:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:07:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 16:07:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 16:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 16:10:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:10:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 16:10:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 16:10:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e7edaddea6f9cb3888ae01d56ba6ad40984adc9e9f0729fe22295c0a727a7`  
		Last Modified: Sat, 02 Sep 2023 00:09:15 GMT  
		Size: 1.2 MB (1199976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f55f76c08a5cc5ab844531e79f012630a454ad19824466081d47e5a560f9d0`  
		Last Modified: Sat, 02 Sep 2023 00:09:13 GMT  
		Size: 4.7 MB (4680564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d155fc7f6fe8f68905821adbaca9f4255191ebb926d82c352e8f071cd1e3c16`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aeff7aa8ca17f7c5baf131a4d4fe35395c4dcb955fed6ee7fbf8f4d0125712`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b86a26a6b362400fbb68618e387c4080cf614e29538fe5e4b551b1898bc84`  
		Last Modified: Sat, 02 Sep 2023 00:09:55 GMT  
		Size: 157.4 MB (157421027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a9b567886dae0363aae1c506920c4cbfc1020ce73865e875ad155ce0af8c3`  
		Last Modified: Sat, 02 Sep 2023 00:09:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f2439b922cac680e8c6cefcb54a18fa0c06efa19f290e0c7106c287944c9b1b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205346052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f02c719ef94496b7e6b92b6f5e381407904a4ca59c2e0b0fd8efc218cea02ae`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:02:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:02:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Aug 2023 15:02:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Aug 2023 15:02:38 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Aug 2023 15:05:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:05:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 16 Aug 2023 15:05:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Aug 2023 15:05:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15340a0f1b3eb99199990d967961a6a7095eccee4a7e4b4a73d5f695318b9c0`  
		Last Modified: Wed, 16 Aug 2023 15:36:35 GMT  
		Size: 1.2 MB (1199928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721226cd510b20bfa5e238d93f0c82d74955fe088f6a76baf10edd313c20865d`  
		Last Modified: Wed, 16 Aug 2023 15:36:33 GMT  
		Size: 5.5 MB (5533316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0e3a60370b22bc9740a59b8aa14fb13ccdff17844a659d622e95eb49aadee`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439f340ca803a67b808daca6069b8332fb18927cf901c22569e32b8fbbe825d`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72576e868a3e7c4d3fc831d20bce9ee1236edd7e6713b812cecc47fa9bdc66d`  
		Last Modified: Wed, 16 Aug 2023 15:37:06 GMT  
		Size: 171.4 MB (171409809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d637f1ed1675da3f70e7ae5fdd2e2f2b82c99cfb4bfeeec599928e70b238651`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:8528d686750fabbbe2159598768afcfa4c2bdc65bec9e0ee0441b5a4c83e02ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:89cbe43679330e6bd5782d41d5399c605810e4e0534722a5f7d259c783ebe04c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268789357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacb7afabee43df46482d7be96a41072fbe81ac929a033222a050d06e6aa400b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:47:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:48:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:48:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d4a6718b1e51ddd8764334554078659b49564a31b2ea34cee00a1c5f437411`  
		Last Modified: Sat, 02 Sep 2023 01:56:04 GMT  
		Size: 85.2 MB (85155757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d89b626f703ae38c08a97d108c79d5c7cad00a1fc192be8a343b8f68dae96ed`  
		Last Modified: Sat, 02 Sep 2023 01:55:54 GMT  
		Size: 296.4 KB (296424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a7eb86e7476d48a099e042ae94ee2f9e4d04e81f448cf71724ae798d40b0dc`  
		Last Modified: Sat, 02 Sep 2023 01:55:53 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2db7d172353485493767f1d6662f6db0350701c9816d3e04067b1425e042980`  
		Last Modified: Sat, 02 Sep 2023 01:55:57 GMT  
		Size: 23.7 MB (23706688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:40cfdd3d89ecf88a0f9228fcffeca26d2c45a1f7670a4e18504c2307c5b4989f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.3 MB (261280765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0594f5593323d6af3a45c4ef0368843cd518e0818d6937647217e985488d53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:40:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:40:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6143eb2220e8d9afb221d0fa655a5077c5f98b5f6a64c4b7bc581df94207d`  
		Last Modified: Sat, 02 Sep 2023 00:48:07 GMT  
		Size: 82.8 MB (82840195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99426183657f085286925e298ba13fe7c3ffdeb4fdaae65eff9e7fa08d3d537`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 296.4 KB (296418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed58b9cae2a1ecd194bbd9e221feb51eab6abd8e334f13d9aeaeab299b9378b`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 2.4 KB (2397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1320cc5b95f582bfb8ee5c8d92da3bc220dac1fbdc8a1de8c5fec4a3243db88e`  
		Last Modified: Sat, 02 Sep 2023 00:48:02 GMT  
		Size: 23.1 MB (23105075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:52e824e68b23f5c29065412b5caa245d5b249eab54362a305c146b8d523a1fbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:c35f3425ec4d468b2db7b10fbba70b407a0464532226d2c488eea1167dd6aa5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.7 MB (959670787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fde0935136cb80fdc66b6c134e911beff0c667adfd07d004a4bb3437b2c15649`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:47:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:48:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:48:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d4a6718b1e51ddd8764334554078659b49564a31b2ea34cee00a1c5f437411`  
		Last Modified: Sat, 02 Sep 2023 01:56:04 GMT  
		Size: 85.2 MB (85155757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d89b626f703ae38c08a97d108c79d5c7cad00a1fc192be8a343b8f68dae96ed`  
		Last Modified: Sat, 02 Sep 2023 01:55:54 GMT  
		Size: 296.4 KB (296424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a7eb86e7476d48a099e042ae94ee2f9e4d04e81f448cf71724ae798d40b0dc`  
		Last Modified: Sat, 02 Sep 2023 01:55:53 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2db7d172353485493767f1d6662f6db0350701c9816d3e04067b1425e042980`  
		Last Modified: Sat, 02 Sep 2023 01:55:57 GMT  
		Size: 23.7 MB (23706688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510705f6838088c76fae685f7142918c63d37febd1d4165ec114c62803ec5670`  
		Last Modified: Sat, 02 Sep 2023 01:57:42 GMT  
		Size: 690.9 MB (690881430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c7ab76d297deded741a05f020c9323390158d6547f696516d3a48b2922753234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.0 MB (920001838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d851028348b73855c044b595f77dace7298c5b554d8bb6124d0db6ef1bf68df`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:40:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:40:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6143eb2220e8d9afb221d0fa655a5077c5f98b5f6a64c4b7bc581df94207d`  
		Last Modified: Sat, 02 Sep 2023 00:48:07 GMT  
		Size: 82.8 MB (82840195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99426183657f085286925e298ba13fe7c3ffdeb4fdaae65eff9e7fa08d3d537`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 296.4 KB (296418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed58b9cae2a1ecd194bbd9e221feb51eab6abd8e334f13d9aeaeab299b9378b`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 2.4 KB (2397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1320cc5b95f582bfb8ee5c8d92da3bc220dac1fbdc8a1de8c5fec4a3243db88e`  
		Last Modified: Sat, 02 Sep 2023 00:48:02 GMT  
		Size: 23.1 MB (23105075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9a5d045635df93719a7f5f6fe6584c7401d864ac59b3d631439d79d98adef8`  
		Last Modified: Sat, 02 Sep 2023 00:49:20 GMT  
		Size: 658.7 MB (658721073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:52e824e68b23f5c29065412b5caa245d5b249eab54362a305c146b8d523a1fbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c35f3425ec4d468b2db7b10fbba70b407a0464532226d2c488eea1167dd6aa5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.7 MB (959670787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fde0935136cb80fdc66b6c134e911beff0c667adfd07d004a4bb3437b2c15649`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:47:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:48:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:48:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d4a6718b1e51ddd8764334554078659b49564a31b2ea34cee00a1c5f437411`  
		Last Modified: Sat, 02 Sep 2023 01:56:04 GMT  
		Size: 85.2 MB (85155757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d89b626f703ae38c08a97d108c79d5c7cad00a1fc192be8a343b8f68dae96ed`  
		Last Modified: Sat, 02 Sep 2023 01:55:54 GMT  
		Size: 296.4 KB (296424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a7eb86e7476d48a099e042ae94ee2f9e4d04e81f448cf71724ae798d40b0dc`  
		Last Modified: Sat, 02 Sep 2023 01:55:53 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2db7d172353485493767f1d6662f6db0350701c9816d3e04067b1425e042980`  
		Last Modified: Sat, 02 Sep 2023 01:55:57 GMT  
		Size: 23.7 MB (23706688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510705f6838088c76fae685f7142918c63d37febd1d4165ec114c62803ec5670`  
		Last Modified: Sat, 02 Sep 2023 01:57:42 GMT  
		Size: 690.9 MB (690881430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c7ab76d297deded741a05f020c9323390158d6547f696516d3a48b2922753234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.0 MB (920001838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d851028348b73855c044b595f77dace7298c5b554d8bb6124d0db6ef1bf68df`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:40:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:40:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6143eb2220e8d9afb221d0fa655a5077c5f98b5f6a64c4b7bc581df94207d`  
		Last Modified: Sat, 02 Sep 2023 00:48:07 GMT  
		Size: 82.8 MB (82840195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99426183657f085286925e298ba13fe7c3ffdeb4fdaae65eff9e7fa08d3d537`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 296.4 KB (296418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed58b9cae2a1ecd194bbd9e221feb51eab6abd8e334f13d9aeaeab299b9378b`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 2.4 KB (2397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1320cc5b95f582bfb8ee5c8d92da3bc220dac1fbdc8a1de8c5fec4a3243db88e`  
		Last Modified: Sat, 02 Sep 2023 00:48:02 GMT  
		Size: 23.1 MB (23105075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9a5d045635df93719a7f5f6fe6584c7401d864ac59b3d631439d79d98adef8`  
		Last Modified: Sat, 02 Sep 2023 00:49:20 GMT  
		Size: 658.7 MB (658721073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:8528d686750fabbbe2159598768afcfa4c2bdc65bec9e0ee0441b5a4c83e02ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:89cbe43679330e6bd5782d41d5399c605810e4e0534722a5f7d259c783ebe04c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268789357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacb7afabee43df46482d7be96a41072fbe81ac929a033222a050d06e6aa400b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:47:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:48:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:48:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d4a6718b1e51ddd8764334554078659b49564a31b2ea34cee00a1c5f437411`  
		Last Modified: Sat, 02 Sep 2023 01:56:04 GMT  
		Size: 85.2 MB (85155757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d89b626f703ae38c08a97d108c79d5c7cad00a1fc192be8a343b8f68dae96ed`  
		Last Modified: Sat, 02 Sep 2023 01:55:54 GMT  
		Size: 296.4 KB (296424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a7eb86e7476d48a099e042ae94ee2f9e4d04e81f448cf71724ae798d40b0dc`  
		Last Modified: Sat, 02 Sep 2023 01:55:53 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2db7d172353485493767f1d6662f6db0350701c9816d3e04067b1425e042980`  
		Last Modified: Sat, 02 Sep 2023 01:55:57 GMT  
		Size: 23.7 MB (23706688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:40cfdd3d89ecf88a0f9228fcffeca26d2c45a1f7670a4e18504c2307c5b4989f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.3 MB (261280765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0594f5593323d6af3a45c4ef0368843cd518e0818d6937647217e985488d53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:40:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:40:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6143eb2220e8d9afb221d0fa655a5077c5f98b5f6a64c4b7bc581df94207d`  
		Last Modified: Sat, 02 Sep 2023 00:48:07 GMT  
		Size: 82.8 MB (82840195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99426183657f085286925e298ba13fe7c3ffdeb4fdaae65eff9e7fa08d3d537`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 296.4 KB (296418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed58b9cae2a1ecd194bbd9e221feb51eab6abd8e334f13d9aeaeab299b9378b`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 2.4 KB (2397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1320cc5b95f582bfb8ee5c8d92da3bc220dac1fbdc8a1de8c5fec4a3243db88e`  
		Last Modified: Sat, 02 Sep 2023 00:48:02 GMT  
		Size: 23.1 MB (23105075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:8528d686750fabbbe2159598768afcfa4c2bdc65bec9e0ee0441b5a4c83e02ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:89cbe43679330e6bd5782d41d5399c605810e4e0534722a5f7d259c783ebe04c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268789357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacb7afabee43df46482d7be96a41072fbe81ac929a033222a050d06e6aa400b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:47:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:48:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:48:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d4a6718b1e51ddd8764334554078659b49564a31b2ea34cee00a1c5f437411`  
		Last Modified: Sat, 02 Sep 2023 01:56:04 GMT  
		Size: 85.2 MB (85155757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d89b626f703ae38c08a97d108c79d5c7cad00a1fc192be8a343b8f68dae96ed`  
		Last Modified: Sat, 02 Sep 2023 01:55:54 GMT  
		Size: 296.4 KB (296424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a7eb86e7476d48a099e042ae94ee2f9e4d04e81f448cf71724ae798d40b0dc`  
		Last Modified: Sat, 02 Sep 2023 01:55:53 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2db7d172353485493767f1d6662f6db0350701c9816d3e04067b1425e042980`  
		Last Modified: Sat, 02 Sep 2023 01:55:57 GMT  
		Size: 23.7 MB (23706688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:40cfdd3d89ecf88a0f9228fcffeca26d2c45a1f7670a4e18504c2307c5b4989f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.3 MB (261280765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0594f5593323d6af3a45c4ef0368843cd518e0818d6937647217e985488d53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:40:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:40:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6143eb2220e8d9afb221d0fa655a5077c5f98b5f6a64c4b7bc581df94207d`  
		Last Modified: Sat, 02 Sep 2023 00:48:07 GMT  
		Size: 82.8 MB (82840195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99426183657f085286925e298ba13fe7c3ffdeb4fdaae65eff9e7fa08d3d537`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 296.4 KB (296418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed58b9cae2a1ecd194bbd9e221feb51eab6abd8e334f13d9aeaeab299b9378b`  
		Last Modified: Sat, 02 Sep 2023 00:47:59 GMT  
		Size: 2.4 KB (2397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1320cc5b95f582bfb8ee5c8d92da3bc220dac1fbdc8a1de8c5fec4a3243db88e`  
		Last Modified: Sat, 02 Sep 2023 00:48:02 GMT  
		Size: 23.1 MB (23105075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:127cfc3636b57faa860e6a807455f876f089e4be89fd9d1ab783bab995010403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:30cc2c2ed3dba85278928dfb03689cc75dd8243de716f4e11f04f691b9b00021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159628079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c37109b0bc864263ba24a9c8e509220721cf92980096816e58a2d6d3f9131120`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ddafd21cc956b87da96e34e4f0ec2fff34d57997ec6629c5e78cca7dbc68e940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155036680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf0b35c84d8c29c0c984a5517450bfc0560552e7534647750c2be8ac03baebe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:127cfc3636b57faa860e6a807455f876f089e4be89fd9d1ab783bab995010403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:30cc2c2ed3dba85278928dfb03689cc75dd8243de716f4e11f04f691b9b00021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159628079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c37109b0bc864263ba24a9c8e509220721cf92980096816e58a2d6d3f9131120`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:46:52 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 01:47:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:47:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:47:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:47:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c83bf7cfb5b1507ccb5c8b29e14df05fbf1c1af286dbdd1a0760341610f1d7`  
		Last Modified: Sat, 02 Sep 2023 01:55:45 GMT  
		Size: 124.1 MB (124144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c207b8c1657762bdcf593d5a5aa230db3d7239a51c6e1e91991c7db355c2bf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ddafd21cc956b87da96e34e4f0ec2fff34d57997ec6629c5e78cca7dbc68e940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155036680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf0b35c84d8c29c0c984a5517450bfc0560552e7534647750c2be8ac03baebe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:39:16 GMT
ENV ROS_DISTRO=rolling
# Sat, 02 Sep 2023 00:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:01 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:40:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:40:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac57ba3d69f161b5cbcaaf5bcb4371f6b36256c810306cfcc4f2c779904f27e`  
		Last Modified: Sat, 02 Sep 2023 00:47:51 GMT  
		Size: 121.6 MB (121622867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f819035049306e4fd5b131a0971c2daff48f95c0c0cc378aec37ab0e1cb291`  
		Last Modified: Sat, 02 Sep 2023 00:47:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
