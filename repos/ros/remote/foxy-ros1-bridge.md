## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:305309d77c82b932b0f39274107f20dace64722bbe74c9594b5708cad2db8698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:a917c84926ec2df2be30f4ae025e4246c1e1040048dc6f4ca2d94147aea88322
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349090769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4ade7aad1eb1539c25aa29307372f260775bcfec5f1058c5f976632452cbaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:13:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:13:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 01:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:13:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:13:42 GMT
ENV ROS1_DISTRO=noetic
# Tue, 18 Apr 2023 01:13:42 GMT
ENV ROS2_DISTRO=foxy
# Tue, 18 Apr 2023 01:14:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:14:17 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275738f8603356f715759926c672904eafa8bfac12a6f4fc1bb25f30a2f2e67e`  
		Last Modified: Tue, 18 Apr 2023 01:18:03 GMT  
		Size: 73.3 MB (73341056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0cfeddf32468988708b8205f0dd73996e224c00857773fa9557bdbfa385e4d`  
		Last Modified: Tue, 18 Apr 2023 01:17:54 GMT  
		Size: 260.0 KB (259961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049fa8b21143456bf6302da9c1f5d27a1c4f9e8b05028511aa67f3bbabd481`  
		Last Modified: Tue, 18 Apr 2023 01:17:53 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a0278b454639d3064fd38db41ae5a3d05e16ffa4bf223b9e78fb59d37f8a6`  
		Last Modified: Tue, 18 Apr 2023 01:17:57 GMT  
		Size: 21.7 MB (21681848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a237f51a7ce837970a1a3147689c6e320812c6e113379b34a4ede309865b9`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099dcbb0d68914ea8e128b9ba5bfd6dc295a0df1df6dee77077e5c41c02fd09a`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f219045d848c72ef970168d3d659ecc472d96ce1ddd0b941afa86e942eeed327`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 76.4 MB (76429430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e95e56ab27365bbf52b85a050085d25498a5cb779cbecc348312453c755ecc9`  
		Last Modified: Tue, 18 Apr 2023 01:18:18 GMT  
		Size: 21.7 MB (21674170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bac345354e272b6a28e6a211fdbe0140442e7945f38f1a4456c97b3c013dd7`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3eb948c5217a16ff7fcfb7d9e22efaf54ab2d16f82cb3d10df0fb492fafd6370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.7 MB (317659720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f76a3adf578db9fa908cb48f4597a414e3c146fed3a0d860dd5b9ee2da5c1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:20:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:20:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 02:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:20:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:20:53 GMT
ENV ROS1_DISTRO=noetic
# Tue, 18 Apr 2023 02:20:53 GMT
ENV ROS2_DISTRO=foxy
# Tue, 18 Apr 2023 02:21:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:21:24 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1542c121861076309738d45ca122ce9226e3ae7b21ce08ab861c95a66c4ed6d5`  
		Last Modified: Tue, 18 Apr 2023 02:24:26 GMT  
		Size: 67.7 MB (67686900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ccb99230453021ceb67c88f4ad0f60b938ad64160c5fb83dbc7349abd6c00`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 260.0 KB (259959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de229310fdd44a856f4c3aa202e5c38eda5342328e3f890fc486b4178be68007`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a74b94f680052b89e94e45989edce2610e247ef9fbd7629c0851d7c04f3d6d`  
		Last Modified: Tue, 18 Apr 2023 02:24:21 GMT  
		Size: 20.4 MB (20406633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f9d68432b2d7450ddf62a0c75dbefc697f27fe5cb8fb1fb52acc60cb96bc70`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8935466a6297cbe16a3d6d8445036f9ffe2ab0078e98a0ad5e737c27444fea6`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ae7d7ef45a74fd1945390dfdaa493a7e91fb43ea0e6b6fa7a4248e8e1c42f`  
		Last Modified: Tue, 18 Apr 2023 02:24:47 GMT  
		Size: 76.5 MB (76496301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df84ef9c108d7326c078732759bbb9ae47b5c4ba4d59e3509127dd8bdf8f9f03`  
		Last Modified: Tue, 18 Apr 2023 02:24:44 GMT  
		Size: 14.3 MB (14325458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21af496781b7139843b526b25641e3fc46797877d26b5ebb0f035710286ea258`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
