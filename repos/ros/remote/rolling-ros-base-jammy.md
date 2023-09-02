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
