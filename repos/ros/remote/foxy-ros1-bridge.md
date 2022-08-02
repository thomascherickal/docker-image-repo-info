## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:f8c5c673dba4b9a2dbba8ba6ee18ccb8d711ae9a42e1ed513eb7de87c94bc527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:26ff0b66e8070fb5883bc6d3e79e429be979ce4fbc5e78f5735ece8ff91cb000
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.6 MB (348611143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbbea4c2c80151dacde3a8b0ffc4e53500e6be19da3c08f93ef911fa2bc15dad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:10:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:10:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:27:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 02 Aug 2022 13:27:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 13:27:25 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 13:27:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 13:27:25 GMT
ENV ROS_DISTRO=foxy
# Tue, 02 Aug 2022 13:29:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:29:19 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 02 Aug 2022 13:29:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:29:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:30:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:30:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 13:30:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 02 Aug 2022 13:31:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:31:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 13:31:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 13:31:26 GMT
ENV ROS1_DISTRO=noetic
# Tue, 02 Aug 2022 13:31:26 GMT
ENV ROS2_DISTRO=foxy
# Tue, 02 Aug 2022 13:32:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:32:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:32:49 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3f991215ddc16cd6d5839a01c05ba58b96914830f35c25d3d72e0495b053e7`  
		Last Modified: Tue, 02 Aug 2022 13:55:17 GMT  
		Size: 1.2 MB (1181319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc0c69710a5bf5069bd2509080fc6d8b47b7f817d02eb6b5c420be6abe69e`  
		Last Modified: Tue, 02 Aug 2022 13:55:15 GMT  
		Size: 5.5 MB (5546864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b843c9985c018b28399cfe7cdf458b105aa857166116387fb59aea69773e`  
		Last Modified: Tue, 02 Aug 2022 14:01:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7d4dffb56dd34745f4b3d35b10fffeaa9fb9d3e4289645c3f872151b5ee3ae`  
		Last Modified: Tue, 02 Aug 2022 14:01:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c52ae16f14310233a6e7249f0fa763fae9f5995610d370d531d882fff1f338d`  
		Last Modified: Tue, 02 Aug 2022 14:01:37 GMT  
		Size: 120.1 MB (120094593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbe4231b7280f383df6653740ce8b62eb7b3b26eb9b73063194fb33adaad0c5`  
		Last Modified: Tue, 02 Aug 2022 14:01:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860d019f8d83ce737fa22bbc20d50e8ad9ee06c8b790aecd7ad5f4f5b7b4217`  
		Last Modified: Tue, 02 Aug 2022 14:01:58 GMT  
		Size: 73.3 MB (73321236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4deaeff6a713d4b6767976eb346827c701fe347d528f6851b6092cdc151c65`  
		Last Modified: Tue, 02 Aug 2022 14:01:47 GMT  
		Size: 260.9 KB (260923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6111214e0f2e935ae823a1da2de08f1d686923dc249d6d4372d640bdbb42e92`  
		Last Modified: Tue, 02 Aug 2022 14:01:47 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eacb7c7081c45f56ff2d971ab52dbff21183ebd2588413f8c7e8a957b2fd35c`  
		Last Modified: Tue, 02 Aug 2022 14:01:50 GMT  
		Size: 21.7 MB (21663296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d636529f999eca09444b318ce3241d317e552f0a4f640b0c1031c9324e7e0`  
		Last Modified: Tue, 02 Aug 2022 14:02:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7c3f4a148e52800a0deda3bb24c15be7027cffdfb1f971d66d6671897590ae`  
		Last Modified: Tue, 02 Aug 2022 14:02:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c665fa6f5986478cebe9e16d9818f4577a2b1579d903cd92409ef63ae5a7b`  
		Last Modified: Tue, 02 Aug 2022 14:02:26 GMT  
		Size: 76.4 MB (76429024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5363e563fb5b79bdebe0877b556c871de06f2c9c6837bf93b788c1191cf8a1`  
		Last Modified: Tue, 02 Aug 2022 14:02:16 GMT  
		Size: 21.5 MB (21535985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a857bad74b67654b2f1ab2d8ffbac122b18319ed2133b987de53f69657798f`  
		Last Modified: Tue, 02 Aug 2022 14:02:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6fd856c54fd98f2437bb25dc38a3e33b6f1d399ba504b9c0254d1bddcca58613
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 MB (316157750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91ecce56c2fbfc182cecf69bf4b6134e04550599fcebdf0362a62a9a92e27a86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:58:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jun 2022 05:58:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:58:12 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:58:13 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:58:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 07 Jun 2022 05:59:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:56:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 11 Jul 2022 23:56:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:56:53 GMT
CMD ["bash"]
# Mon, 11 Jul 2022 23:57:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:57:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 11 Jul 2022 23:57:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 11 Jul 2022 23:57:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:58:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 11 Jul 2022 23:58:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 11 Jul 2022 23:58:05 GMT
ENV ROS1_DISTRO=noetic
# Mon, 11 Jul 2022 23:58:06 GMT
ENV ROS2_DISTRO=foxy
# Mon, 11 Jul 2022 23:58:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:58:53 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba1af7accc591a88c8a5f7fcf1bf476eff87854e2eac51402705fb2a99e6d`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de599d7de9bc16e737c7d0bfa8e04fbc3af9a6e8c01427667056cf9b535382b`  
		Last Modified: Tue, 07 Jun 2022 06:20:40 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cdbf24e724491ae84bce273d36577ddf420bcbb4080a8280e8fa98fdede28b`  
		Last Modified: Tue, 07 Jun 2022 06:20:58 GMT  
		Size: 104.3 MB (104273904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7f425745113f9e4ee736d38d7eb2c7b2dbb9e2dd07f5dc0c152a4100082b02`  
		Last Modified: Tue, 12 Jul 2022 00:16:30 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea0746cc02c6916f9b617fc2f009bdcc79cd8dbaca9965980392588d496bab0`  
		Last Modified: Tue, 12 Jul 2022 00:16:50 GMT  
		Size: 67.4 MB (67440079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df9a82cec08fa5b2af57fdea5ae9752e59b030c76a7db7b6d4aae3959146c05`  
		Last Modified: Tue, 12 Jul 2022 00:16:41 GMT  
		Size: 260.3 KB (260264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbbed0a71e55e8f2782361ccea22f9069d1d28ea8d8f72600e31f9994d2ce2f`  
		Last Modified: Tue, 12 Jul 2022 00:16:41 GMT  
		Size: 2.2 KB (2207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691577d09729b48191ac7513b4e09873d02f5fca637b871d864bd74cb1edf1d8`  
		Last Modified: Tue, 12 Jul 2022 00:16:44 GMT  
		Size: 20.4 MB (20365694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da2e814a15fc3f9f09b486fa58ae07bd37a297a6d3da50da2c2429cd819ac00`  
		Last Modified: Tue, 12 Jul 2022 00:17:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02604ee353174d089c643832e409edba4ad501ac0342acd7ef04cfb58212764b`  
		Last Modified: Tue, 12 Jul 2022 00:17:20 GMT  
		Size: 76.2 MB (76159201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5951b38461ee47250874fe5039b9a0d3fc2924b0c4d624ca9cff68372bc0f`  
		Last Modified: Tue, 12 Jul 2022 00:17:08 GMT  
		Size: 14.0 MB (13956800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6772fed2bb5ad49b0b13f53d15a7d50deebe3d2d8f56759758a8306ebf156d5c`  
		Last Modified: Tue, 12 Jul 2022 00:17:06 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
