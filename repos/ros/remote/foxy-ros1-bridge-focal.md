## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:6e5504e7240a4719023081dec783080a8f558ce1aa39f35fb9576ec0783202cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:f6f5c0a0e4853ebcb1d0c793d490da59bd2d64e6a5f872210082b42730db3f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.7 MB (349716175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0977093e1753c1bf7fb7338dbbbce5e7fe7a1baee3a2b24ab01af46d236e91f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:37:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:37:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:37:08 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 03:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:06 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:38:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:38:06 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:38:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:38:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:39:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:39:14 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 03:39:14 GMT
ENV ROS2_DISTRO=foxy
# Fri, 22 Apr 2022 03:39:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:39:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9020050231a832ea7ec08f8436054efcd6e8a4d4ff6650fa51af143b21e723`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad51f3ba74c73756f5c46e18fe955db3d8a6a7ea0457271430340cb811b85`  
		Last Modified: Fri, 22 Apr 2022 03:52:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e452458b64576978a29ec3371779b11068f93fb9c221ab69945e5c619ac2bd37`  
		Last Modified: Fri, 22 Apr 2022 03:52:44 GMT  
		Size: 120.1 MB (120084788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab9a02fbc2fb68fd882c39887a0d9650772448527ff6fcaa3d0f5c55274778`  
		Last Modified: Fri, 22 Apr 2022 03:52:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e6663cc7e7891e966d7dceec6d5a0b5514de61fb1d6a7bf484ef91a686c48`  
		Last Modified: Fri, 22 Apr 2022 03:53:06 GMT  
		Size: 74.5 MB (74539616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11483942dac1171bec761bd7edc1858b665ca4d6eb10be1f55d26f251bdd8e3e`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 254.2 KB (254168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a449ba3ea7f9f55f6e49fd90d40fdb8d928abdf760083c6f239ff44274761`  
		Last Modified: Fri, 22 Apr 2022 03:52:55 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddd03f832a092dd75d894aaf0dc3031bab4f643254329841d41a0f446918ea`  
		Last Modified: Fri, 22 Apr 2022 03:52:59 GMT  
		Size: 21.7 MB (21669649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b5f330b17bff3b79078ad4a779b74b71742d53f1bd9cb4bf256ab89fe6d3e`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308cbc359a788776e176402454db5b48e363e38d8fbbcb052472da3aac8d9206`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea5382ebe2ec51b07e3e93c6d68facc813a488754b27f195e36931889ddf7`  
		Last Modified: Fri, 22 Apr 2022 03:53:36 GMT  
		Size: 76.3 MB (76324782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c672e567bbdbc2ec09e3bf6b2f3e362e0a23eb023827223ce11a4463938b298`  
		Last Modified: Fri, 22 Apr 2022 03:53:26 GMT  
		Size: 21.5 MB (21544441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1febcc87ce4e65c78a1ec45e36df3fa2099f9b70f8e76560cb9db11e7c769834`  
		Last Modified: Fri, 22 Apr 2022 03:53:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:695bd97e5fb12c16202e36da61191fe713ff2147ec22b12f0f31f1247b205ee2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317361780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033c4c76d50f082c86ab16441b0145598eddcb5e4d0b9ae80b8f4efb79750e58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:08:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:08:14 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:08:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:08:16 GMT
ENV ROS_DISTRO=foxy
# Fri, 22 Apr 2022 04:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:09:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:09:15 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:09:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:09:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:10:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:10:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:10:29 GMT
ENV ROS1_DISTRO=noetic
# Fri, 22 Apr 2022 04:10:31 GMT
ENV ROS2_DISTRO=foxy
# Fri, 22 Apr 2022 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:11:25 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb5416a0c308e16e0bcba619713ad8d977de04ee4268d018d1a4dd3d4bb0c4`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e51134f761a8bd21c1e815666d4ae02c2785a2b72a4956cacfba4950bf9c3da`  
		Last Modified: Fri, 22 Apr 2022 04:24:29 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256932324d9f1a02ca236677c33cba022aa3ff2cef91030e79ac875447ef8fe`  
		Last Modified: Fri, 22 Apr 2022 04:24:46 GMT  
		Size: 104.3 MB (104265887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8811f7513053531aa7614b9aab9c2e1035bee15d84aa4865f20d1367210c6653`  
		Last Modified: Fri, 22 Apr 2022 04:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f005082924dedfd2c2f74b7bbac369b39c3019e336021d08d5568beb6175a8`  
		Last Modified: Fri, 22 Apr 2022 04:25:07 GMT  
		Size: 68.7 MB (68670891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf24db3183ac5840e9fb241eefd598017e1484c2b0fba0a7ef31fca05089eb6`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 254.1 KB (254108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececf303279db2d366f0987f68f3eac1211a5688952d26b80860d4ec84af332d`  
		Last Modified: Fri, 22 Apr 2022 04:24:57 GMT  
		Size: 2.1 KB (2127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2b6525381e970f32820151e8f053ec745232a3bfd58600bb3808f28059d19`  
		Last Modified: Fri, 22 Apr 2022 04:25:00 GMT  
		Size: 20.4 MB (20373691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d1a8875302bc9d8a9c3e4061ee2ab7fbcaf59d55558650697341e3a352bcd`  
		Last Modified: Fri, 22 Apr 2022 04:25:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b72035e559f367a7be9a0d6dff792faa3991f692cbba74968ea9e80a0e626d`  
		Last Modified: Fri, 22 Apr 2022 04:25:41 GMT  
		Size: 76.2 MB (76154125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435a6ce1a0bfebd525543e64b85ef20039c3967cc6ca6e9bca0d351a2288854e`  
		Last Modified: Fri, 22 Apr 2022 04:25:29 GMT  
		Size: 14.0 MB (13964662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5aff43097bc70c117dae8f182a5e6c6cfbf1a439b2d8baef3e3349936ffd4f`  
		Last Modified: Fri, 22 Apr 2022 04:25:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
