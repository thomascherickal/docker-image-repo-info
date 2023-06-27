## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:74597f742fef50e0e7a48a458c71fbf17cfd7890db6420fdd5d73a9b6e9dc7c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:9d0acaacfce96d3b1c5aa7898e2b8bc7a6587ac4eeee69773a6f3b1a0015c88e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.6 MB (484642252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0291940e7dea4c037d871136cea40984dbd0fbf02db3b5a3b11c84c5f3bd8f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:19 GMT
ADD file:54838b3dbf7839dadd0b29835bbe53ecbfdfde657ef8671ec5ac3cf5867ea069 in / 
# Mon, 12 Jun 2023 23:21:19 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:08:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:20:49 GMT
RUN echo "deb http://snapshots.ros.org/noetic/final/debian buster main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 27 Jun 2023 01:20:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 27 Jun 2023 01:20:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jun 2023 01:20:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jun 2023 01:20:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jun 2023 01:22:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:22:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 27 Jun 2023 01:22:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jun 2023 01:22:53 GMT
CMD ["bash"]
# Tue, 27 Jun 2023 01:23:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jun 2023 01:24:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:24:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac8bb7e1a32398e26c129ce64e2ddc3e7ec6c34d93424b247f16049f5a91cff4`  
		Last Modified: Mon, 12 Jun 2023 23:26:48 GMT  
		Size: 50.4 MB (50448512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cf5c15547519baec38e96827f04dc5f08cfb702fc8765dfa47ba9b8eb2bd`  
		Last Modified: Tue, 13 Jun 2023 17:17:32 GMT  
		Size: 10.9 MB (10897084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ca51b4c58c0584ed69a618914b0b2c4f50f9d813aa45705d26d84487111652`  
		Last Modified: Tue, 27 Jun 2023 01:36:31 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed4c52cac8a0cefc5f1c09a110eceba6c8c2dd67b0794fac78a8a76c6eab152`  
		Last Modified: Tue, 27 Jun 2023 01:36:31 GMT  
		Size: 3.2 KB (3221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06558bc538997bfde288afa7ad8dc75a26bf86a173687d8ecb4835c1604a1ed`  
		Last Modified: Tue, 27 Jun 2023 01:37:02 GMT  
		Size: 239.2 MB (239247831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac4de4055bb55cdced21af8b9bd8d7208db93781433edb09ec77f762f66a4a7`  
		Last Modified: Tue, 27 Jun 2023 01:36:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9714d55b15206374694f43dbc5e14012e3d3958561691cc600618b51c602a38`  
		Last Modified: Tue, 27 Jun 2023 01:37:21 GMT  
		Size: 86.6 MB (86625286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de079f7ac705565208992d4833c64a6afee5a1f34a9b2438b3008590ad5b22df`  
		Last Modified: Tue, 27 Jun 2023 01:37:10 GMT  
		Size: 296.7 KB (296668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328d719d1ece58de5bc6fe76401e990484678c5b27587fae7ba29c19fc41c074`  
		Last Modified: Tue, 27 Jun 2023 01:37:20 GMT  
		Size: 76.0 MB (75965659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733b07889b02fe8b69f6b8d84960dad8a6261ea4d84b7ed8e962d2cca781a54`  
		Last Modified: Tue, 27 Jun 2023 01:37:30 GMT  
		Size: 21.2 MB (21157566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:38ff97dd0b170409e3a0bd4fd4b287e05c8906a2a472f30e8ff3363eb430ba06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424270809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f80e202b527263e97bac6d884bcc789565884d3ae05373890f3d324397cc703e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:41 GMT
ADD file:bb3cb9e6abc423742d7c1b6bc006a7cef70038c5621c71a90a2ae7c1ea29ec63 in / 
# Mon, 12 Jun 2023 23:40:42 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 13:42:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:14:45 GMT
RUN echo "deb http://snapshots.ros.org/noetic/final/debian buster main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 27 Jun 2023 02:14:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 27 Jun 2023 02:14:47 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jun 2023 02:14:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jun 2023 02:14:47 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jun 2023 02:16:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:16:35 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 27 Jun 2023 02:16:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jun 2023 02:16:35 GMT
CMD ["bash"]
# Tue, 27 Jun 2023 02:17:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:17:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jun 2023 02:18:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:19:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8371d57f7426517aead21bff5af0cf321625cac166c86214c439fb67db84243`  
		Last Modified: Mon, 12 Jun 2023 23:45:01 GMT  
		Size: 49.2 MB (49238409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03375f4355e227cafbfa908999c3ddc516dfece8850f794cbfee3d98a3b0e4d`  
		Last Modified: Tue, 13 Jun 2023 13:51:27 GMT  
		Size: 10.9 MB (10902698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45b1051edd106997caba4f1579a4b2d4504d49a9f038bd54e527ed3c6af1f20`  
		Last Modified: Tue, 27 Jun 2023 02:31:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69434a5448d8f4de484bef98eebf3d4c5b06d3e23a551a42d2ffa417bfccaa9b`  
		Last Modified: Tue, 27 Jun 2023 02:31:54 GMT  
		Size: 3.2 KB (3220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d304c38e18c1dc16bf7685a133b35ef5a4146eda4daf5588d8e10614644dc11`  
		Last Modified: Tue, 27 Jun 2023 02:32:16 GMT  
		Size: 184.5 MB (184467829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb2d67a4b4053020362b7ffdebed6f8cdcfc288a27b86a226d683d27bb74c3`  
		Last Modified: Tue, 27 Jun 2023 02:31:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c15492fc212e032c0c600760c3010cfa16e5e1f3effedf32d06a3cb20c50234`  
		Last Modified: Tue, 27 Jun 2023 02:32:30 GMT  
		Size: 84.4 MB (84396678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41b1f1feee5807337977c61f98f8cbaeac56b4abee9717800664a743b3113f2`  
		Last Modified: Tue, 27 Jun 2023 02:32:22 GMT  
		Size: 296.7 KB (296671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97231e066b5561577be394ddb64afad8e6751213826298539935e9fc1721b3b`  
		Last Modified: Tue, 27 Jun 2023 02:32:29 GMT  
		Size: 74.1 MB (74135945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f83ed58f623dc9e54eb594a6677cae672b306fa2c2f5e75d4ff04758af5007`  
		Last Modified: Tue, 27 Jun 2023 02:32:38 GMT  
		Size: 20.8 MB (20828935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
