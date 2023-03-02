## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:7e1c2380af8e1974a811309152788066b26b0009c7d2773aafef6f94c6bf8d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:ff6c79a978b1675cbba65b8dfad9911c0ae2393c4cec127bd57cacfbd110165a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212300650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1790d729b37324de7ce9b8987b25473dcd9f1ada37ab2260676a91f950f4eab1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:45:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:39:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:39:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 20:39:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 20:39:50 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 20:39:51 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 20:39:51 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 20:41:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:41:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 20:41:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 20:41:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db143da9f5a088b47cfbe87905f9e615f3b537f906257fc11ac7a38ffb0f236c`  
		Last Modified: Wed, 01 Feb 2023 18:58:42 GMT  
		Size: 1.2 MB (1154526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52bb4834a5fa25fa5b39cba579b1676bc6fc585a61819ffad44865e1f80e40`  
		Last Modified: Wed, 01 Feb 2023 20:55:33 GMT  
		Size: 5.6 MB (5553686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec367e72b62793708adc92e14601369a3c38859319b9863f10e9fa9ba932a7a`  
		Last Modified: Wed, 01 Feb 2023 20:55:32 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87879323c6acc8c68e6878f4c6747f5b19224e5ab7d3565ae982d5cec4986e0b`  
		Last Modified: Wed, 01 Feb 2023 20:55:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87260597f032f87f0f5afdfa9e7af5532c34f19a268badac9a326f79fdc0e5b`  
		Last Modified: Wed, 01 Feb 2023 20:56:01 GMT  
		Size: 177.0 MB (177012139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49267a4c47886ecd6f474669d8dbb6885d4765902c1474912ad1e74ab9929f89`  
		Last Modified: Wed, 01 Feb 2023 20:55:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:384f19f5099a3865f3447b895af7e748be7453ab036d8a8ae0ac6d86c371ebcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187935561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a14468079f6c5d9c96ce30eb310845d1c67d556d44cfc2d8bc5d5c2485aa6e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:75b39f2eb13e7db3653d56e63728799a3e25c6bf7868c6b02318922fbe17e7d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205370200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ae095b06299fee387b279f3f2e0ed1f4eabe255a73826905e51bd7b9aa1575`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
