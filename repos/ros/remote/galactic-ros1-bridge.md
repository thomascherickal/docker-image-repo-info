## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:e3e0491163cf62ebfee428213292ad1cc26566f0b2db95f4eb48befb2bfc3040
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:147cab728b6776ab4f956f0bfd307ac8646af9c61107f93ad54549bee15642cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.0 MB (330039447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b0f4fbe76b9774aaaff171e8a868d82675e13cc4ae26fd93b3725bc5cd897`
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
# Tue, 02 Aug 2022 13:33:02 GMT
ENV ROS_DISTRO=galactic
# Tue, 02 Aug 2022 13:33:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:33:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 02 Aug 2022 13:33:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:33:45 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:34:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:34:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 13:34:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 02 Aug 2022 13:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:34:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 13:34:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 13:34:40 GMT
ENV ROS1_DISTRO=noetic
# Tue, 02 Aug 2022 13:34:40 GMT
ENV ROS2_DISTRO=galactic
# Tue, 02 Aug 2022 13:35:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:35:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:35:17 GMT
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
	-	`sha256:dff5bc0f4410a9a4df17b2ba68d11b669ca1b5bfeb7de939c97e51d05b1b4dae`  
		Last Modified: Tue, 02 Aug 2022 14:03:03 GMT  
		Size: 103.9 MB (103883299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a0c156e3f431ed899d85555fd6240ce1d49f9a40e54350b529a495823808f`  
		Last Modified: Tue, 02 Aug 2022 14:02:37 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2bd50d7d05880919f8f6a90f132ff76c104c3edea5258199b2387889dc84a`  
		Last Modified: Tue, 02 Aug 2022 14:03:26 GMT  
		Size: 73.3 MB (73278242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d06c0f29101913e5f40d7fc33f4c270f9b4ef2279944a5308711d28664e4fca`  
		Last Modified: Tue, 02 Aug 2022 14:03:14 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469a75f80a7f31bd5d819c55b008a36b5ac2069f8fa30f2cc7ea08afa5525a34`  
		Last Modified: Tue, 02 Aug 2022 14:03:14 GMT  
		Size: 2.2 KB (2226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bc9b7ea12109f91d10341166fd078867c43304721c1f6a88e0c9e5de0f8dce`  
		Last Modified: Tue, 02 Aug 2022 14:03:19 GMT  
		Size: 22.1 MB (22132816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e2f251f1be18e9fb2b6db36330a52f23588ca3fe197df909d52e01bbaf7ed2`  
		Last Modified: Tue, 02 Aug 2022 14:03:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b47309acdec21a52ec827e96d46c35254586a1424edd6f99a7f158f7a329f2`  
		Last Modified: Tue, 02 Aug 2022 14:03:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e5c11db36799f600e24665cd1af78a91ec3c7aaf994390b56441ca3ad91d5`  
		Last Modified: Tue, 02 Aug 2022 14:04:00 GMT  
		Size: 78.7 MB (78703374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14e3868dbd8a3c44c7419b1384ebe2dbc7f455a0d433a11230334d736eed6a8`  
		Last Modified: Tue, 02 Aug 2022 14:03:43 GMT  
		Size: 16.5 MB (16463831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c634d47e9ca1f1b831cc123df1c366c3e694c0eaa33d27e57e988278f5c72a8b`  
		Last Modified: Tue, 02 Aug 2022 14:03:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7307868e185451773a7dcdd208ac1d5c87590d382bff220419e89d9edfe6d6ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.2 MB (319191450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0436931c64829593faa84faa05c17ee9f2a70e3f8b51c6c643bcb950b2bda271`
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
# Tue, 07 Jun 2022 06:01:24 GMT
ENV ROS_DISTRO=galactic
# Tue, 07 Jun 2022 06:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:59:03 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 11 Jul 2022 23:59:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:59:05 GMT
CMD ["bash"]
# Mon, 11 Jul 2022 23:59:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:59:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 11 Jul 2022 23:59:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 11 Jul 2022 23:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 00:00:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jul 2022 00:00:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jul 2022 00:00:15 GMT
ENV ROS1_DISTRO=noetic
# Tue, 12 Jul 2022 00:00:17 GMT
ENV ROS2_DISTRO=galactic
# Tue, 12 Jul 2022 00:00:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 00:01:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 00:01:05 GMT
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
	-	`sha256:45025b4c3908f5af9c9a4562800e13737a9d64436d4921a61e77eb06ce9d36d8`  
		Last Modified: Tue, 07 Jun 2022 06:22:18 GMT  
		Size: 100.3 MB (100299397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43434c2c4bf4a9d1242279f72a2e62ab35041d7aa84cd079ecc46a811f90f735`  
		Last Modified: Tue, 12 Jul 2022 00:17:33 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f9fae1de6cc90dc59e2a4530cc5a385af707745c1af9d18fb1631b2d616d53`  
		Last Modified: Tue, 12 Jul 2022 00:17:53 GMT  
		Size: 67.4 MB (67391927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4727d441bd369009c099e7653d2b46e14deaef5255ea226be5ff95fcc17b9b`  
		Last Modified: Tue, 12 Jul 2022 00:17:44 GMT  
		Size: 271.1 KB (271077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce88d6c5986ba9310ee5c65c1582a636c916d2afe1d18e384f6bfea066e7e6`  
		Last Modified: Tue, 12 Jul 2022 00:17:44 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a774d280c626b294f9c30ddb8c793f49732dfc848f8a129c774390ef8c63ba8d`  
		Last Modified: Tue, 12 Jul 2022 00:17:47 GMT  
		Size: 21.5 MB (21453104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3af50e0e51ae31aafb0b00760ca9c701d23d1efdaa459aa8de6e95d39b47c4`  
		Last Modified: Tue, 12 Jul 2022 00:18:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5812f759690bd3a9d31275501b21e191a5f00740c27d0502b17983949db70c05`  
		Last Modified: Tue, 12 Jul 2022 00:18:25 GMT  
		Size: 80.3 MB (80312540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c35a42b882c8ed8a968242e8210ce1613224fa9d10b83eac6d700bd06315c0a`  
		Last Modified: Tue, 12 Jul 2022 00:18:13 GMT  
		Size: 15.8 MB (15761621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b40c9105f7c6a0170e38715131de21af3a4f1e8a6cf8fd002c1d6719f58dff`  
		Last Modified: Tue, 12 Jul 2022 00:18:10 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
