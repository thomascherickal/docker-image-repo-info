## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:64a4306900ab63eb44b93ba66c6ac3e0bede2b83cf85586049caf9d3aa881a3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:08388a8f291a61bafc049a98bafc9c2ef2a7a58f3909cc90d67b98a1f7bb45b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.0 MB (968013134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a3b0467f6eb0d92bf3c16db06cb5a90993e6b1ef764947e6d64b4b3079627a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:54:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:54:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 14:54:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 14:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:55:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 14:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 14:55:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:56:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 14:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a25b8c075beb4891f7c9088956d2a452f32036d8126e37217b5b62fd7024c`  
		Last Modified: Tue, 17 Aug 2021 15:02:09 GMT  
		Size: 10.9 MB (10891952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b43ac20734a706cb03369661415e15f6856a48275dcd4fe7744b0bde5d23`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b19825ce46253a4664a6e606382250ba22ec8d0e1d13516be7d225efcca57f`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034eef40d3fabaea23b5d4473263a3a6ab8cd3545504c1ba16818b3b90152d1f`  
		Last Modified: Tue, 17 Aug 2021 15:02:50 GMT  
		Size: 239.1 MB (239050839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae7d371ba1fee4f46bf91b9a18289de1dd3472eb2c3b8458f8ff2df5825c78`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b4384fc4992e164b0946674e8bf7905f6037fbe56d20552b0a9f981e0b23df`  
		Last Modified: Tue, 17 Aug 2021 15:03:21 GMT  
		Size: 86.6 MB (86566411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6466d96361536da7163da2fbe6e4e5267a768c30f1f04480d818c767e0ef32`  
		Last Modified: Tue, 17 Aug 2021 15:02:59 GMT  
		Size: 310.1 KB (310086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43da0dad1381eb1948df8e9a05518d305a6b3a7df20eb1f0b82edb2a00bee76b`  
		Last Modified: Tue, 17 Aug 2021 15:03:19 GMT  
		Size: 76.0 MB (75975146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b682f5f1680f2c4ec265e9f6da30a3f02e3e8782fbb3f6ced55263d693845a`  
		Last Modified: Tue, 17 Aug 2021 15:05:05 GMT  
		Size: 504.8 MB (504780085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b125f0aa8c4f4c983c9a2d4f86fa924bb3213ce72f437e7c9cd51e3ed6231c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.8 MB (884790908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0df7b3716b359e1fef891e626df838827f22961f2d578af5470027d5395e506`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:27:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:27:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 03 Sep 2021 11:27:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 03 Sep 2021 11:27:50 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:27:50 GMT
ENV LC_ALL=C.UTF-8
# Fri, 03 Sep 2021 11:27:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 03 Sep 2021 11:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:28:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 03 Sep 2021 11:28:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 03 Sep 2021 11:28:50 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:29:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:29:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 03 Sep 2021 11:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1462dbe8ebf1cb3c2f5806cb19d8c66f38c095230d7abce37bddb2ba968ca5bd`  
		Last Modified: Fri, 03 Sep 2021 11:35:40 GMT  
		Size: 10.9 MB (10883319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2664a95765076375c283614578526207643956bf3842410bcc7bf4d68dee1862`  
		Last Modified: Fri, 03 Sep 2021 11:35:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b32b930665db018324ae169bf319ec4667a22080016cfe417f1c301a301bb`  
		Last Modified: Fri, 03 Sep 2021 11:35:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b848e0f07ce6baab097af02bd4e576eb86c8e1b06351507016049cb42b6631d`  
		Last Modified: Fri, 03 Sep 2021 11:36:12 GMT  
		Size: 184.2 MB (184239824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0fa9131028a94f4fffe644b96939f628590f4295592695f28746a9e10984b`  
		Last Modified: Fri, 03 Sep 2021 11:35:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b96c7e42a14a58819a5bb3314a6f83b3626344879f544d27813fb33a8ed36e2`  
		Last Modified: Fri, 03 Sep 2021 11:36:33 GMT  
		Size: 84.4 MB (84358204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae83f3620e550f184b0f2548271c264a849e7c8f8925a1ec8d6cf06b06e12f4`  
		Last Modified: Fri, 03 Sep 2021 11:36:21 GMT  
		Size: 313.3 KB (313339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aad3176387dcdd01db7601abcb3321fc3ba932666dd79a8b225e297b96d426`  
		Last Modified: Fri, 03 Sep 2021 11:36:31 GMT  
		Size: 74.1 MB (74087922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8507d540be8d1bdac423987942a18de5eec31fdd7232e8d79b4c8a30f30480`  
		Last Modified: Fri, 03 Sep 2021 11:38:08 GMT  
		Size: 481.7 MB (481683748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
