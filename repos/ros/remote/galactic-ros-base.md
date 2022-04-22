## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:05ff07940a5ed666b30f0e9cb3e5989e3d0af92393950351c418c5ccc8703137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:57982240c0b1d9639b5d4017bd39fd04ffb6e1947f059b9bb2c46320879db806
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235830367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf1eab5ff47ea02c884e6f99e01b82106247185704ba244505d93fa6ec51b75`
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
# Fri, 22 Apr 2022 03:40:00 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 03:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:40:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:40:43 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:41:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:41:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:41:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:41:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:8a86987c94783b7f050791cd972e66bdcf20ee12dcccd1a0162756a9bbea3ff5`  
		Last Modified: Fri, 22 Apr 2022 03:54:05 GMT  
		Size: 103.7 MB (103662159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3e7c02467d0b63472d97b71a8664755cfe96d8fe8c6842a7b4861910bc761`  
		Last Modified: Fri, 22 Apr 2022 03:53:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d81b4f14257aafe9c36754217f7b33e5594f7991bdc5fed442f3e351818ca6`  
		Last Modified: Fri, 22 Apr 2022 03:54:26 GMT  
		Size: 74.5 MB (74494199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86ee117572ea9ab37045a8143bd74f2c6fc866407f2c1b855fef3c348bec9f6`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 262.2 KB (262250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc056e4b5fb80b3e3a36e14d46061812f16e11166015dfbf5c8e9f911b4bc5e0`  
		Last Modified: Fri, 22 Apr 2022 03:54:15 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a725f33deb8c6696fb2fe8f21c3fe0f20e6598f23354c10b3d1953701fe651`  
		Last Modified: Fri, 22 Apr 2022 03:54:18 GMT  
		Size: 22.1 MB (22113636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:226fa8b063571c73b4edede044f3a5c5dd59c24dcd749be5af219ae29ab60229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224032026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea80bb6394b0a866f1da8a2d6bbf18c448a676b6ac18e4c23c17c3926c256d41`
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
# Fri, 22 Apr 2022 04:11:37 GMT
ENV ROS_DISTRO=galactic
# Fri, 22 Apr 2022 04:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:13:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:13:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:13:27 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:14:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f16a5650aa4b55dc971dfe0fceffe3fc3812b527dfc4157039f1cc9d11aa34da`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 100.0 MB (100038664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c592e87609fbae5b76ca6ede7467c9310403ef4750a8bdb838445c36429bc85`  
		Last Modified: Fri, 22 Apr 2022 04:25:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04358f3e939d7f9f6a53c0ecd2c599e6321d2b4b0c0e9978c2dc6f05632e9711`  
		Last Modified: Fri, 22 Apr 2022 04:26:32 GMT  
		Size: 68.6 MB (68617910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cf32eefb7bf397b5f31ea8c519a7b26f428c65adf974fcbef5723a3b4d940`  
		Last Modified: Fri, 22 Apr 2022 04:26:22 GMT  
		Size: 262.2 KB (262191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dcc8fe6b031dddb7ee69684824d72831849927f310d7a78c509de355dc75e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:21 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad2443021a6726dfc79be4f57e7f0f6ee1ff0584377c492703e027d379c085`  
		Last Modified: Fri, 22 Apr 2022 04:26:25 GMT  
		Size: 21.4 MB (21435296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
