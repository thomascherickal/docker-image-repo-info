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
