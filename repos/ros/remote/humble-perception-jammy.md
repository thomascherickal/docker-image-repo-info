## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:1369b7c5d308c65bf3ad5832fc1aa7a95516c1ec5b993467813efa3d3489db93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:1140315bd15e40bc9ffc0565c8d53175beaf5bfa24bf25ec8d09784399a944d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1086568827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58a0ace6c3ceb5c9a6fcd3b781d39d498119eaca4b0fcef6192ba157d33edc53`
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
# Tue, 02 Aug 2022 13:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:400e7013c241689097f8df1159db9317a7aaa68c6a2798340cad47ea5a69cc49`  
		Last Modified: Tue, 02 Aug 2022 14:07:11 GMT  
		Size: 823.8 MB (823814828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:735632dea7862da67ed8f40f4dc3e601e049e5e3c57d120e3ad67ab31fea8216
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034770213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ce1d7f2981eb221ca9adf1e8ddf2caebd57e6e8edc092fff39486a856c98d7`
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
# Tue, 12 Jul 2022 00:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:81a2a517132684fec18094e584ae8d51f478cf3dc4030509e2cb997248a71fc8`  
		Last Modified: Tue, 12 Jul 2022 00:21:02 GMT  
		Size: 779.8 MB (779817762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
