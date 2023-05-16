## `ros:melodic`

```console
$ docker pull ros@sha256:4c16420fc4f1f71dd59278ea8f881eef389cb3d9417faaa12edc6553615d767d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:21bb4ad490af560bb44192eed50c1c493358c59c01d70171814c9afbec151bbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437749392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77f179e2e80523fb74868ca6cc6d867b9fc5131cdeb36db2e4e9f1fc9ea0e2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:0deb73ef8cdb24db1b6e38252bdcd582b97c120df9883c5e2d92c29503d1080a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386361722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce96880b22806db09af180be813a22b103b113db2f5cb686151ae7b771b0c4a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:598eef934e9a0771c770be071bd381472cc667fbdd566290db95cf6d1448656d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a267fa349af659c76cdfb1f050f322f0584799eddf7902aa2bf7b22944db4a82`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
