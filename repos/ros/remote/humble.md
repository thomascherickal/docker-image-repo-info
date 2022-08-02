## `ros:humble`

```console
$ docker pull ros@sha256:79a03d998b0bc40edfb565421ab40bde1c2c342034b5c7e3da948e90a97e2040
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:e3f310e9de945ad756d03d0f2609e5ed8415bca86c08f6e57e65d23da982795d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262753999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bb33e15a008f880229bac48f5056f5dbb3d3764ef55c0801a7880138e76a9f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:35:41 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:35:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:35:57 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 02 Aug 2022 13:35:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 13:35:58 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 13:35:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 13:35:58 GMT
ENV ROS_DISTRO=humble
# Tue, 02 Aug 2022 13:37:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:37:39 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 02 Aug 2022 13:37:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:37:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:38:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:38:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 13:38:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 02 Aug 2022 13:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5bfc5848603bd668295b5a975d71c189291f87f6598cf6dc5205c57efdc41f`  
		Last Modified: Tue, 02 Aug 2022 14:04:13 GMT  
		Size: 1.2 MB (1192245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c425ff1dadf43c340925189568bc8f392e60eec7d53b401bb72a710aa66135c`  
		Last Modified: Tue, 02 Aug 2022 14:04:11 GMT  
		Size: 3.8 MB (3827758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43eae6de5e53443906b64a12ebc086b149ea851be37c5c514c6a4b7d1446ac6e`  
		Last Modified: Tue, 02 Aug 2022 14:04:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b619038cdfe7b8c10e6820e8ebbfc5b3ab2e7bff0008f9498e10f48a3948ca`  
		Last Modified: Tue, 02 Aug 2022 14:04:10 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b149af5857de5b95b05668990bef7749088ee5e72afac8e34e07edb55b26f2`  
		Last Modified: Tue, 02 Aug 2022 14:04:35 GMT  
		Size: 106.2 MB (106164552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292f52350cdcdfef6bb772303448c6d04258cef179310be8711a9b3f13cc4dad`  
		Last Modified: Tue, 02 Aug 2022 14:04:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d5567e60848fa47d516eccb165a83b9ba0e3ff50df104d90de5f4d8c1f540`  
		Last Modified: Tue, 02 Aug 2022 14:05:00 GMT  
		Size: 97.8 MB (97848680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123c6566c81129cd717b77b7656fdff7655520e8d6ca726554e3617f9926872a`  
		Last Modified: Tue, 02 Aug 2022 14:04:45 GMT  
		Size: 283.0 KB (283034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18091009f452ed85ae96624f6d932f8350ecafdedda1cc70e3d7ef55a044460`  
		Last Modified: Tue, 02 Aug 2022 14:04:46 GMT  
		Size: 2.2 KB (2249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388e81439f28e9eb3612a6c4f5d7c3f4538cb052e151c5017a4b507a1174d4ea`  
		Last Modified: Tue, 02 Aug 2022 14:04:50 GMT  
		Size: 23.0 MB (23006931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9ea91e710075591699df092e1b55d19f01c330d552fb1896a5dd0d78c43e7cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254952451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec44e1257961dbaaaaac727554c0b393a881a8267388248d38e91d3f7c076e35`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:04:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:04:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 06:04:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 06:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 06:05:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 06:05:01 GMT
ENV ROS_DISTRO=humble
# Tue, 07 Jun 2022 06:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 00:01:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 12 Jul 2022 00:01:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jul 2022 00:01:15 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:01:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 00:01:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Jul 2022 00:01:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 12 Jul 2022 00:02:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b38f97e6001c6a08e3dc9944afe7213ac786bed47db29ee11755c6040f4eb0`  
		Last Modified: Tue, 07 Jun 2022 06:23:22 GMT  
		Size: 1.2 MB (1193148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e937b319a974108dac2f8e36b8f73cd96710ce7663bdf1f72284fccd43df6abe`  
		Last Modified: Tue, 07 Jun 2022 06:23:20 GMT  
		Size: 3.6 MB (3595011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1effce9a47b0ec30acadccc8c075e64e320b43af40a3600dbac215a9d94b87`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da9dba47edebe9f3610145826c05ead7b35e702981de104853623ccc5208fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfb35f5e4a5b9143c3d9046c7a959e8e235ba7491b4f03bb5647ece48cc7fd`  
		Last Modified: Tue, 07 Jun 2022 06:23:36 GMT  
		Size: 103.9 MB (103862447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7663bad4b6ef7946cb336eb33e19d7eada577092dbd480f17e1172b458555c9e`  
		Last Modified: Tue, 12 Jul 2022 00:18:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c7e86d021fbeab4380c654352555c8349dc20c45735409cfb9c9a2e4c380d4`  
		Last Modified: Tue, 12 Jul 2022 00:19:01 GMT  
		Size: 95.2 MB (95213852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4be91b2ec52eef2fc4051fd46d099f581d6adc11d8621f3272ee66242b800b`  
		Last Modified: Tue, 12 Jul 2022 00:18:47 GMT  
		Size: 280.2 KB (280208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468ac5d63f70fcbe3dff272c6580d83e29a588136b0cb99a7d07dfac61d7f655`  
		Last Modified: Tue, 12 Jul 2022 00:18:47 GMT  
		Size: 2.2 KB (2198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45923a67bd26362f8fbb20d87caed755d7e601e09edc06fbb04d5b321bc5affb`  
		Last Modified: Tue, 12 Jul 2022 00:18:50 GMT  
		Size: 22.4 MB (22425001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
