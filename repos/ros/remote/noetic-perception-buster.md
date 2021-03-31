## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:5020fbd0176251f7656daf5d2add822d96bfa16c02e2d116bbc8d6a2ba3a9527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:da86d429c0b4db202c2649a895bf701f8456df52a5b52f084a728f6317aaadd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **967.8 MB (967834499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5e0b6fb06dd6f06875c97893b515a847b6b0e8a46d424b99ab166e2e9496f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:41 GMT
ADD file:89234bb2f86c7eb890235a48904d1c9898a8d287a525c4fe5698d4a04cdd8f12 in / 
# Fri, 26 Mar 2021 15:20:42 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:18:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:19:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 27 Mar 2021 09:19:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 27 Mar 2021 09:19:01 GMT
ENV LANG=C.UTF-8
# Sat, 27 Mar 2021 09:19:01 GMT
ENV LC_ALL=C.UTF-8
# Sat, 27 Mar 2021 09:19:02 GMT
ENV ROS_DISTRO=noetic
# Sat, 27 Mar 2021 09:20:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:20:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 27 Mar 2021 09:20:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 27 Mar 2021 09:20:07 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:20:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:20:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 27 Mar 2021 09:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:24:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bf9c589d5f9475f1fcc050e02308d6b4eeb86eab7752ef948a13693e81a6aaa`  
		Last Modified: Fri, 26 Mar 2021 15:27:11 GMT  
		Size: 50.4 MB (50400278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f449035c3af90c31ff21aac54677ddaa94af7b4199927b2f133e67e8595890b`  
		Last Modified: Sat, 27 Mar 2021 09:29:31 GMT  
		Size: 10.9 MB (10891856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456137ab974bca1d8f62d7d5680410744326ca834b1a0b28f08439320b0760e6`  
		Last Modified: Sat, 27 Mar 2021 09:29:28 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1385d40e15645e2c90531a6509af986cdf1443339297d7fe19d8279b932c5ca`  
		Last Modified: Sat, 27 Mar 2021 09:29:28 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb71cc1ea410520d668b783bdd3e0a1a5c7b5f781d4adc019127c0b6c76a3f1c`  
		Last Modified: Sat, 27 Mar 2021 09:30:24 GMT  
		Size: 239.0 MB (238991317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886c7fa5d1013621ff1cbf8d90848d0ccd58d5769abfb273e8a5760ea7cbdd10`  
		Last Modified: Sat, 27 Mar 2021 09:29:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09ce8b79379dd299aa16f768d61fbecdd248503ba14153c488473212c646325`  
		Last Modified: Sat, 27 Mar 2021 09:30:49 GMT  
		Size: 86.6 MB (86566359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac64f5538503a14d3bfde99b870e7313c132f18a63f039d615ebac954589ed`  
		Last Modified: Sat, 27 Mar 2021 09:30:33 GMT  
		Size: 274.0 KB (274003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaf0f42bd10ccb191c0271e1ed66a9a8a47b8abcf30bcb9e13c6a33eea92abf`  
		Last Modified: Sat, 27 Mar 2021 09:30:45 GMT  
		Size: 76.0 MB (75974718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eeb49e2de36bf3ba49502f688292dc2e71a44f96e16b035a4cc42015476fde2`  
		Last Modified: Sat, 27 Mar 2021 09:32:33 GMT  
		Size: 504.7 MB (504734131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:73e5c9268bdcf46ac7113342225b358029486bf84eaa89f92166352ef668a5ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.7 MB (884655379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f1289979a68dd15a6428fe3a8bc6b319d26c6e3a67e0be3d0c855c052d634f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:49:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:49:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 31 Mar 2021 13:49:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 31 Mar 2021 13:49:21 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 13:49:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 31 Mar 2021 13:49:23 GMT
ENV ROS_DISTRO=noetic
# Wed, 31 Mar 2021 13:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:52:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 31 Mar 2021 13:52:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 31 Mar 2021 13:52:37 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:53:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:53:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 31 Mar 2021 13:54:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:00:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10597693b224937ce4d457543a06dce5f11624a25fa61e62534b154013a92a`  
		Last Modified: Wed, 31 Mar 2021 14:08:28 GMT  
		Size: 10.9 MB (10883525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c008f3dddbf040a2e694f39105725834300ae8f8477c9dbbd5c79b5cb23199a`  
		Last Modified: Wed, 31 Mar 2021 14:08:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add46ffbec133da5c01b9a88e9e3989183c864f9619f612cde268cb3c36438bd`  
		Last Modified: Wed, 31 Mar 2021 14:08:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574e6d0cf1ff497632a742787107585220c26cabe302cb5bd891ab5baa174f94`  
		Last Modified: Wed, 31 Mar 2021 14:09:49 GMT  
		Size: 184.2 MB (184204230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843b94776c6c910590000e226121d2215ae485328207fdde890c502a6534b73c`  
		Last Modified: Wed, 31 Mar 2021 14:08:25 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630b0c397b1e57dd750dbb39bf40b5b90c14f4d033e3f5d8eff5a454038643f`  
		Last Modified: Wed, 31 Mar 2021 14:10:17 GMT  
		Size: 84.4 MB (84358908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c435ce95597dbc5279339cade8cd740061c12cca6b61e3be9d4bdeb5d84e625`  
		Last Modified: Wed, 31 Mar 2021 14:09:57 GMT  
		Size: 274.8 KB (274834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e702c0310f7256e54459711a324685c55275c8471b1138e525692b2aa5c9bd`  
		Last Modified: Wed, 31 Mar 2021 14:10:14 GMT  
		Size: 74.1 MB (74089164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baa98ee54570149903dfde957b905737f138d1297b0361e945f3fd51468639d`  
		Last Modified: Wed, 31 Mar 2021 14:13:01 GMT  
		Size: 481.6 MB (481617071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
