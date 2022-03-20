## `ros:noetic-robot`

```console
$ docker pull ros@sha256:e4ca720faaff237039849a82bd4a1ee9ca4c2da83c2d05b7c78d152300141c49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:6d77a6f2215d20a4f7a43e37fc9c38cd20eedd1d9ee0c87c980ee99930116ecb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358876553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e89738f4b762f6bde05ebc574ea3b1de6951a75d7930fbd1bdb56844ff3a87a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14b3d178340a142f77be930235205eba0cbb20d38f959c60b80bafcca9a2396`  
		Last Modified: Fri, 18 Mar 2022 10:03:23 GMT  
		Size: 15.9 MB (15858692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:dcc26aed86d745e75f74b0f20f00593688e2b3f5ea7a6366a1aa1a172ab802cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302700588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3478fe0ec1f8032569256444f4a62e516a6da81bdbcd269497c59fae5068c70`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:05:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0431b613bbb09218e76bd77919289ac304de70f5a8298da508929c92d87c0b`  
		Last Modified: Sun, 20 Mar 2022 07:23:32 GMT  
		Size: 14.1 MB (14063319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8c32e120858113e11f1b32171bb6023f7d53557b3ba50070e26fc9190f8657ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337490786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9799d75786b5d247442b54801332512161a3038e4d816e494c96582dde6a228`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:55:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bc39db48f396854215b5422c9a3ebf01e6ee06216501b6f8496b9b9f356e9`  
		Last Modified: Fri, 18 Mar 2022 01:22:38 GMT  
		Size: 15.4 MB (15447361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
