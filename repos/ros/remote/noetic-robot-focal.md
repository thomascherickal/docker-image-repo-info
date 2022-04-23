## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:d53671120c79755fc3bc654b8984e155b1902736cde6bbfa7dd10e629c49f877
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:82adffa092e98d53cac94a9ecb55ba7569efc8f0f5d22fa619f93ce70eb50a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358880748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e0ca8e38ae15069727b4c1507435dfe3fb53c865c6ab323f807fd32afdec7f`
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
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f093d22dbe5877606fa8a0bb7ab4ff9f764a797720db05f3891f492ba89135`  
		Last Modified: Fri, 22 Apr 2022 03:50:46 GMT  
		Size: 15.9 MB (15858801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:cc8b94ba7be48707d801a8625d42f5719f34ace16f442de9b409a4da99645dce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302721758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3be1b316388d7521caddb1b63790c6f62911e0e387087508a86d6a014ea2a41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:03:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:03:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 01:03:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 01:03:23 GMT
ENV ROS_DISTRO=noetic
# Sat, 23 Apr 2022 01:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:05:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 01:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 01:05:52 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:06:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:06:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 01:07:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:08:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1c5853014fa7b45d7fffba9d88224220b84ba829f662ce9e4ad6f876cd5c4`  
		Last Modified: Sat, 23 Apr 2022 01:22:07 GMT  
		Size: 1.2 MB (1182227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a8bdfc415bd3eeb2b576469686696ad5a7afcca2db8b9347ecda0fc5154838`  
		Last Modified: Sat, 23 Apr 2022 01:22:05 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624aa88c80df0eb9d8d6df667fa30112e087ad9b36d5ee692ab1131c1283d24`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63735cc8022aa53a46d8f008fc41c23a5b395f6c487d5ee242b8e5eabe9e6a7`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b72edc6bb57f6c8efd09814017260434105711df1530437d16593c4ebb6a27`  
		Last Modified: Sat, 23 Apr 2022 01:24:10 GMT  
		Size: 157.4 MB (157423209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621cc883afe0018a1c5b202199b38c99b52da70d61d2e07b3aef83eeb200bd0`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe19da18d443e06bab72c5a422dd2eb3d8329a923a3a09d29896e72a6dad25`  
		Last Modified: Sat, 23 Apr 2022 01:24:46 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5885ff5921c1504d714951d416752d525b8df2852ab16def36205521f67fc6`  
		Last Modified: Sat, 23 Apr 2022 01:24:23 GMT  
		Size: 315.3 KB (315274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11816648be3079dae038d3ef403e655297636aee161db9a4f83ea04b7ffb0cf7`  
		Last Modified: Sat, 23 Apr 2022 01:25:02 GMT  
		Size: 60.5 MB (60482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8713ba4b0281ed1eed08b6b88dd2382461ef68e4919ad6e671af93353b37d5b9`  
		Last Modified: Sat, 23 Apr 2022 01:25:28 GMT  
		Size: 14.1 MB (14064446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e688ed73e138f25890349e5090c1c3b0c970ce916148b160d74bdae7f87174c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337482921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b02bf96a11e1a6d842331a5bd039931f13a1c2437d6169445c1feb2d4dc56e1d`
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
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:05:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ad38acc3207d37bdbd042778978ce56aeb0844496c6d6b4fbe085abcd61151`  
		Last Modified: Fri, 22 Apr 2022 04:22:54 GMT  
		Size: 15.4 MB (15447730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
