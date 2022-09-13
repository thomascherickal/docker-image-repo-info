## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:59bf1634bd79fcc5d1ea8d2681f4b694154cf15fd3a9f38a12500826a5feae04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:5b95a6e605843dc2eb28230f7dd99a304d116f820aa70a8c695d6a8fb0535f7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.0 MB (484951958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa43e500da5c54ad36d7ca8c29bdf5fbdec8bca045751ce9575101b5cdf83c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:21:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:21:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Sep 2022 12:21:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Sep 2022 12:21:22 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 12:21:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Sep 2022 12:21:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Sep 2022 12:22:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:22:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 13 Sep 2022 12:22:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Sep 2022 12:22:32 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:22:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:23:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 13 Sep 2022 12:23:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf49330e6dcf4631b745f36390b6924eb52faae3ca4914217e00162bc6c68356`  
		Last Modified: Tue, 13 Sep 2022 12:28:00 GMT  
		Size: 10.9 MB (10893556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b84e60758dcc196c2a43988dc174dd7bd73986a0b408d81c15f2e4a6e0175`  
		Last Modified: Tue, 13 Sep 2022 12:27:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cdeac817655f3902a59a9aaba2a64e30b481f0d568014ad88b358c952c86b7`  
		Last Modified: Tue, 13 Sep 2022 12:27:59 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755c74d4c66edd4c0e0ef512b7283105748b0bb49535591e26bdcdbd0da47303`  
		Last Modified: Tue, 13 Sep 2022 12:28:32 GMT  
		Size: 239.3 MB (239296126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d4c11830d9370e64c516d2974473ec5b9d5e51353531304367a1150f122ff`  
		Last Modified: Tue, 13 Sep 2022 12:27:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a05071916eb0582b265682c97297c38a1f9137403bd963887113e2b11034e68`  
		Last Modified: Tue, 13 Sep 2022 12:28:53 GMT  
		Size: 86.6 MB (86571688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12ecc199fd0d8a607922d5ffd2ff778dee50f09ae8e17ddeec59a58abcf2f1c`  
		Last Modified: Tue, 13 Sep 2022 12:28:40 GMT  
		Size: 322.2 KB (322244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d60bf49d7534d939a3060e678e5a8f9ae23569995f0ad7e18f8a9b203a2f6b2`  
		Last Modified: Tue, 13 Sep 2022 12:28:51 GMT  
		Size: 76.0 MB (75976937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368d632092b6a3d4533ffb73fa24a18b4c27daefb6079350e4aef754ca0e9284`  
		Last Modified: Tue, 13 Sep 2022 12:29:07 GMT  
		Size: 21.4 MB (21448620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:121b3e7b2ca5e8da32dfd01553c6ac1900af316462c74b3d1e9e796edb3aa97e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (424049494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b246b8ee8dc3e0e2b08a175ccb03cab632821d038b2c68104063a478f2f6db59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:06 GMT
ADD file:304a544562f139d7ab96511b7f1e059966cf90169117e835072f132468bf91c8 in / 
# Tue, 13 Sep 2022 02:11:07 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:56:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:56:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Sep 2022 12:56:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Sep 2022 12:56:44 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 12:56:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Sep 2022 12:56:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Sep 2022 12:58:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:58:13 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 13 Sep 2022 12:58:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Sep 2022 12:58:16 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:59:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 13 Sep 2022 12:59:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:00:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2406a452ad23ba9085e0708f5e15309206a618eb828aa307becbb239414392f`  
		Last Modified: Tue, 13 Sep 2022 02:16:42 GMT  
		Size: 49.2 MB (49228261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ec060bafb85a1c4fb32a456ed970628f926c8b985fb90ed243d4c7d4d96d6f`  
		Last Modified: Tue, 13 Sep 2022 13:06:39 GMT  
		Size: 10.7 MB (10689346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f272eefce84866a380e21ef07b830d72077f566702b1dc8432c9bd460423b18`  
		Last Modified: Tue, 13 Sep 2022 13:06:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4d36aa5f5718c160f03a683078a7a6a33c621f22763243a6cba5a31fec922`  
		Last Modified: Tue, 13 Sep 2022 13:06:37 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4b761086d86c468aad5c1c5a5a8b2904284754e9efa06d510edcc4b50a638`  
		Last Modified: Tue, 13 Sep 2022 13:07:08 GMT  
		Size: 184.5 MB (184463015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15616e1c2e135cd3c48087cab44685dcd6953ceeb63f92b3ae64f09578961f44`  
		Last Modified: Tue, 13 Sep 2022 13:06:37 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00b67bbdb5f9e8d9d7db843b5b3004d079a09724f3ac83c20eead20bcb6536e`  
		Last Modified: Tue, 13 Sep 2022 13:07:27 GMT  
		Size: 84.4 MB (84371420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee5988a175290b2b265a5b3255b001f45b42ac83f55aa18d418183c2ee5507f`  
		Last Modified: Tue, 13 Sep 2022 13:07:17 GMT  
		Size: 322.2 KB (322186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583b0ab9e5f1ddccc929af774d99cf94fc8cb22ca41e734283678b1dad875c36`  
		Last Modified: Tue, 13 Sep 2022 13:07:26 GMT  
		Size: 73.9 MB (73865756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b28d909643f86dd58e2f1738edd414e9ab03785021a60e39d8296406b1c7b12`  
		Last Modified: Tue, 13 Sep 2022 13:07:38 GMT  
		Size: 21.1 MB (21107140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
