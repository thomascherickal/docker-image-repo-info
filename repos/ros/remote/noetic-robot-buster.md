## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:830b8b6b228f8b58a80be1d71531ce1f515e8aaa5d6a5a85a872eb9ea41003ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:33469620b61bf346857ea107808f9b6490c4c053877906144f4bc06c492626fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.0 MB (484032615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf7f349468ed21495000bf29975c6dce97a35822d3b8c761641311a3b0f2f985`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:52:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:52:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Aug 2020 06:52:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Aug 2020 06:52:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 06:52:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Aug 2020 06:52:22 GMT
ENV ROS_DISTRO=noetic
# Wed, 05 Aug 2020 06:53:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:53:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 05 Aug 2020 06:53:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Aug 2020 06:53:25 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:53:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:53:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Aug 2020 06:54:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:54:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91563a4363bc60194f754cd55795c0bdfd23e4f12bea50c0b292fe358d804b57`  
		Last Modified: Wed, 05 Aug 2020 07:05:18 GMT  
		Size: 10.9 MB (10889327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5545a9d65404a1ec0f4ff1975cb1e36517cb1d3802322aad3431ab80904851f5`  
		Last Modified: Wed, 05 Aug 2020 07:05:17 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a6b1162c9ea2f144147436037369d117fa022b280ca47916332d60261d2aa6`  
		Last Modified: Wed, 05 Aug 2020 07:05:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385b447fa489face0db0cc3e93da19b0ce94793a5ffee49fa58430ab4db43c0e`  
		Last Modified: Wed, 05 Aug 2020 07:06:08 GMT  
		Size: 238.8 MB (238837794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92df0de08e6899d24b543e9bbc6149bb2edb3dace806003b21a59de091c8b766`  
		Last Modified: Wed, 05 Aug 2020 07:05:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3a303e5f36b6f9e3a9a51c68b6340eac0f78baf627eeacbbbcee6ccf9677d3`  
		Last Modified: Wed, 05 Aug 2020 07:06:29 GMT  
		Size: 86.6 MB (86563387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308844e1aa8521ee17afaa75cf33ac4532600f2653696f7dff40983a785917f`  
		Last Modified: Wed, 05 Aug 2020 07:06:12 GMT  
		Size: 211.6 KB (211617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de64a72d41978d089c929cb781e0c291b3e7e838f6106d192079e6cfad3d7847`  
		Last Modified: Wed, 05 Aug 2020 07:06:26 GMT  
		Size: 76.0 MB (75965133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc9d94c236cc79f53494d3d735484e913f46a1cfd3577cba3adedc201781fc`  
		Last Modified: Wed, 05 Aug 2020 07:06:36 GMT  
		Size: 21.2 MB (21167521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fde10c0934128f3390b3f469f0378bd6c35a0d0b62453b0a7ecb25ca0cd21be7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.6 MB (423599606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217718c2d7a358c3563d68c56d64b70ac832a07cc31716d7da3c98741927f053`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:16:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Aug 2020 10:16:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Aug 2020 10:16:29 GMT
ENV LANG=C.UTF-8
# Tue, 04 Aug 2020 10:16:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Aug 2020 10:16:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Aug 2020 10:19:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:19:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 04 Aug 2020 10:19:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Aug 2020 10:19:44 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:20:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:21:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Aug 2020 10:22:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:23:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1e3fb9bc333a926aec0d0bd3fd71d27371bc8eee253902e8c37133a1387cf0`  
		Last Modified: Tue, 04 Aug 2020 10:35:22 GMT  
		Size: 10.9 MB (10882026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292bab18c0d540bd5284459808c3310d802d50ae0abd31163f7d5b610424739`  
		Last Modified: Tue, 04 Aug 2020 10:35:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6918466f489333df325cc01bab8c768887c8d7d799b3049f6693172c7c2f5`  
		Last Modified: Tue, 04 Aug 2020 10:35:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598e4c72a6a58a3a062e73876dfc3af1c41fce791679e367ec49a7d1803fee5b`  
		Last Modified: Tue, 04 Aug 2020 10:36:27 GMT  
		Size: 184.1 MB (184069980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bfa31468fc59d35b1dfa798d96d8124b2d711e844fec9f4eca42b2b18d0e9c`  
		Last Modified: Tue, 04 Aug 2020 10:35:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3abfcbb2f5b21e9158901c82def3138ee0abaec2065c266f65644f630683ea`  
		Last Modified: Tue, 04 Aug 2020 10:37:02 GMT  
		Size: 84.4 MB (84354661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65320f532c15eae3952d71c00e835e6146b10173c6685c9fb881e82e8a37aaa`  
		Last Modified: Tue, 04 Aug 2020 10:36:35 GMT  
		Size: 211.3 KB (211304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2ad80aec0a86d16cd10849469c185220827e370f505219e9f285239d9d99a9`  
		Last Modified: Tue, 04 Aug 2020 10:37:01 GMT  
		Size: 74.1 MB (74088257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c320260d10e07fb43b89e7d588d6425422eb1d4b1d27a85b55d20f8c34da41`  
		Last Modified: Tue, 04 Aug 2020 10:37:14 GMT  
		Size: 20.8 MB (20816047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
