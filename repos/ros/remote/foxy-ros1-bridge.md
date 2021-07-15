## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:ccb6732ea22333c2027ed771d46b29a08cde9d96c7cbc2fae9a382e5792a06d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:1d6b89577432ca2593141f7c0753f2ab0ae062cf9987d9f9c4e440f290b3c872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345498966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4028ccf5e28817b3038d03f2b422e92a55b53c019d3112cf0aee9a67a4beafa9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:22:58 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:22:59 GMT
ENV ROS2_DISTRO=foxy
# Wed, 14 Jul 2021 02:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:23:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:23:40 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e347f15045e3e88d4ad189addc66be81c4c63316255d777b898a13d20b4744`  
		Last Modified: Wed, 14 Jul 2021 02:36:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac25308bd6733fea269c23e8c098517fef5f615dffd23ef7de28fcc4d9bcb8`  
		Last Modified: Wed, 14 Jul 2021 02:36:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f0b730b7fc10217137ff01e118be98061ab6d2ad0bcd36d54a46a1af3ec0e`  
		Last Modified: Wed, 14 Jul 2021 02:37:00 GMT  
		Size: 76.1 MB (76123398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63af41c6faaa55b9f2ee8e449a74ce20f9f11f32fc1dd0394356e9fb8c2437cf`  
		Last Modified: Wed, 14 Jul 2021 02:36:47 GMT  
		Size: 32.7 MB (32735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f21aa5ee8fbbe32d95305938c99daa615bee725625c4128c438b596bf631d`  
		Last Modified: Wed, 14 Jul 2021 02:36:39 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eb65f9806e158f725ec1a054294296ea093dbef7325110b5e33637abc5e64a3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314018847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86881289b194f2f9681ec937a2d8bbbee046461ff503e09842b6bd0bb51460c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:38:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:38:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:38:17 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:38:17 GMT
ENV ROS2_DISTRO=foxy
# Wed, 14 Jul 2021 00:38:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:39:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:39:09 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee855d2693cfa3c761f057e595d952f3ad9aa28baec4fdb6c7c6aeccebe5253`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c771a7d94ba5d8af44e03039cf751b24155eae28d23719588728df573466ec3a`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0225905d7fa4ba83b5c82c7276fb856b5a60056229687c75ed8f7a862dd5a5b`  
		Last Modified: Wed, 14 Jul 2021 00:56:08 GMT  
		Size: 76.2 MB (76152200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ef894e724d511fd316fd252172ad77ab6c931f19686507871ff43a2d62505a`  
		Last Modified: Wed, 14 Jul 2021 00:55:51 GMT  
		Size: 25.1 MB (25109348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7b814322b4878b354087da9e952e45c63772416117a07772baedd7d5239ff0`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
