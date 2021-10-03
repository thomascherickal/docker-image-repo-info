## `ros:noetic`

```console
$ docker pull ros@sha256:43bb3962354d2732cae4b364e6c70c633eec35b80ab74caec3e2d92d5ffe2f7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:ccaf1b2477838808d73663f41c34719386ad7ea977091fdcbd19c95b9feff8c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339184977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c618f40d6ef1b8f46c2c5e4114809283344e4b751a46ab67c77aa17f174d411`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c1565b2b554d775f1fb2fde93d1aaf76554a6a98d06f10432b0dd4ddd5d6a11c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284625592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c993c90a1323ad3433fb15eda104672fb8cb76cbb6fa74302440f5d1cce65be3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:58:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:58:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:58:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:58:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:58:49 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:58:50 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:58:50 GMT
ENV ROS_DISTRO=noetic
# Sat, 02 Oct 2021 23:01:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 23:01:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 23:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 23:01:18 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 23:01:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 23:02:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 23:02:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14f7601933a719707ac73474fd36b594e276ec05f124eede4583c00a3765e1`  
		Last Modified: Sat, 02 Oct 2021 23:17:32 GMT  
		Size: 1.2 MB (1183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190759aca25186f4350589ec2379c048f06acc06e6a76add5f07ad85349cddef`  
		Last Modified: Sat, 02 Oct 2021 23:17:31 GMT  
		Size: 4.7 MB (4676677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb443648c34995aebe11b76cf0d88b3d5dbe6ff9be3c83c8244667064590838`  
		Last Modified: Sat, 02 Oct 2021 23:17:28 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28459a73b301e7e1c27e687cb740c9d563eaed9cef73d695c8a77376859e5c29`  
		Last Modified: Sat, 02 Oct 2021 23:17:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb581201f743ccc94ea003df789c3399cddf3921206f3a9cf7f973aa4d8343df`  
		Last Modified: Sat, 02 Oct 2021 23:19:37 GMT  
		Size: 157.2 MB (157198799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3977e3e4c004dc13e37f0a979ff077455eca88b6de80ca426deda959062729d`  
		Last Modified: Sat, 02 Oct 2021 23:17:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d645de0dc12b7fb6a0e7145f1b5d5bb3b2dbfb0ef32e570354bdd0852a1d3c2`  
		Last Modified: Sat, 02 Oct 2021 23:20:08 GMT  
		Size: 36.7 MB (36691652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae98c5f7ed3f19c41a02bd80fd99e9ae72b1d0da5c9e679532520992da696e8e`  
		Last Modified: Sat, 02 Oct 2021 23:19:49 GMT  
		Size: 322.5 KB (322459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c514bd37315e66d420577173b75b8daa390059223e7a5c24fdbe7875246f37`  
		Last Modified: Sat, 02 Oct 2021 23:20:29 GMT  
		Size: 60.5 MB (60482719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:66791732edf7e13167d9ea961d962152e5401ffa9d9ceb0f8c2cde65aec974f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318822332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78083a3273027cb4a7fd2603e6461c20f176f7f1dd44e1527c6b8236af556ced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
