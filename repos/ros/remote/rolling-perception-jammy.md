## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:f34b007ab7c0cb04e1ce0cff50a2f1415409be2c6bf435e3022e866bb51af303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:6151ad7951a8781a34c97c005ce05f403078c7dcca16d706d9eef1093f61f1a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.9 MB (959929356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0718394ecbcd8ce13296e31b6308cf467656cdd700dee924fec354b7d5f5f5cc`
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
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 10:02:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 10:02:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 10:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27dc4d0e1602dc1a995fb217537671c6672edcaefd875900cd6b95529e18b50`  
		Last Modified: Sat, 16 Dec 2023 10:13:01 GMT  
		Size: 85.2 MB (85171231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021430433a34f30f7577dc457480693a19277a672e32f30e122942183191eeb`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 302.4 KB (302360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192c516049c2ce35141ccefea9e40cf1312dbcf5328bd09c11706615aef6a66`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 2.5 KB (2476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1682439cc7c141ccfb75c63904f7b22f1930482b24f40000a074c36065060`  
		Last Modified: Sat, 16 Dec 2023 10:12:54 GMT  
		Size: 23.8 MB (23778395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57a4afd56de5507b6b4e4f069caaa8f53b58bae8cedfda1bb72aec1ebbc3043`  
		Last Modified: Sat, 16 Dec 2023 10:14:38 GMT  
		Size: 690.9 MB (690918503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4848289bf828700f36ca27dd9ee027cb7a924cc2b7eafcb911f806a36d28a247
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **924.3 MB (924328458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace7eaf9ea07c3d1c369a8905bebb825bde9bdc5ea181558c8d3e34a801d5033`
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
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:47:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572c203fb61638e5b00d3de9e3bac0f4b598f4fde21a6f77f5771cca8a857d6`  
		Last Modified: Sat, 09 Dec 2023 04:13:18 GMT  
		Size: 82.8 MB (82848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766998918be38f758abf9473673311fbd57620dfcc63ff003401bf793f9d04ef`  
		Last Modified: Sat, 09 Dec 2023 04:13:09 GMT  
		Size: 302.2 KB (302206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6ef4858e91a47e949495aaa6c7f8513680c0713bc96e7782e28528d59238e`  
		Last Modified: Sat, 09 Dec 2023 04:13:08 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a62cc9bcd00dda0816010e2e73b5442c2f81f59fed40a75fd6e18d3cc9539`  
		Last Modified: Sat, 09 Dec 2023 04:13:13 GMT  
		Size: 23.2 MB (23165376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab690d250573851195fd7fc3985e017fb5f1ae136e8ca590d98606b894d55795`  
		Last Modified: Sat, 09 Dec 2023 04:14:51 GMT  
		Size: 658.8 MB (658756800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
