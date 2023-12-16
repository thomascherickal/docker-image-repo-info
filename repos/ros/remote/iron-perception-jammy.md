## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:bcd36bae7318f3436acb69eac6a8743115921a7f462d3b4ac898a5e08d88d1e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e926a73e3f0405ff83c056b15e47288986bc8b1d0e6ab66d0ed8a015bdf7c52b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.9 MB (959858189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721af958086dac84e13f416af1405bb2d2c12371212513c33e113c714d749d94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:59:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:00:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a40dddb0bee6467345aa781b5fb8366bbfbdf8894179f22d2679c94c45c6a`  
		Last Modified: Sat, 16 Dec 2023 10:10:37 GMT  
		Size: 85.2 MB (85168507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047eea6c49b7300964d5e5711df092f29f4f6ef54c9e4335ca993e47bae7875`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 308.8 KB (308838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f6bd3d7020613a1a62f7efe6a2010043b1600b6a5d741c6a5b83bc74b81a`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb861d9d15bcceecc4139716116c4ee9613074610f98a0ca183f6742e78ab5`  
		Last Modified: Sat, 16 Dec 2023 10:10:30 GMT  
		Size: 23.7 MB (23732538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec15ff624c6c9d63e9cc9d0e4c73890c1222f51715f61c93fdc99ea23781359f`  
		Last Modified: Sat, 16 Dec 2023 10:12:14 GMT  
		Size: 690.9 MB (690944208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ece6680e424bb2f3c17e92b7edb69414132e89970e13bd9bba3468bab29d2744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **924.2 MB (924202619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2449f31b251d4a948ed05d90617ed5f465198917f9da8309a31ed9c165bbff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:42:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:42:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12195a3969755cede1841333ad86c88205d160a792081abbe6eb597be1513882`  
		Last Modified: Sat, 09 Dec 2023 04:10:51 GMT  
		Size: 82.8 MB (82845353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd78deb6203197c2d6b1b64486c1f43e4082daea5b1dddb08d735e9b118d401`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 308.7 KB (308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd95dc58fecd704a011c00b89936ba693fa704fcae6c6d66ccd85d0fe88931`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198c81f08313430c71a7721ea05a6ecb30d03552e69d14c08e92d7903cf86e8`  
		Last Modified: Sat, 09 Dec 2023 04:10:46 GMT  
		Size: 23.1 MB (23119813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43178b7bb093094c03a37ce41185b297031fdac6e082a8b2f3dfa1ee3ba911b1`  
		Last Modified: Sat, 09 Dec 2023 04:12:25 GMT  
		Size: 658.7 MB (658731781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
