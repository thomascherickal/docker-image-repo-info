## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:a9909aea5bce2166f90217eda45cfa864d269393a018a03d3981ba5a1ce154de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:261bbee43c8fd92629d856290c1da7cdbadd93d1c53f1ada35da619d6e8097c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.4 MB (951402354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359f68e189ef08d52bd84491269cd0d07683a112cb6e037af121e743fb6af517`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:14 GMT
ADD file:647206e0e9c1daa306e4ebbdc26c3ef1840dd316ba4ffea905d17b0858e58e34 in / 
# Tue, 02 Aug 2022 01:20:14 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:22:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:22:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 13:22:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 13:22:52 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 13:22:53 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 13:22:53 GMT
ENV ROS_DISTRO=noetic
# Tue, 02 Aug 2022 13:23:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:23:57 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 02 Aug 2022 13:23:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:23:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:24:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:24:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 13:24:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:27:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e6a53d1988fa8e19db6bcfc96ee6783afb079c38dbe047528e691815d19a9fa`  
		Last Modified: Tue, 02 Aug 2022 01:24:34 GMT  
		Size: 50.4 MB (50440980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5785ad494f16fd45414b77fd2e2429ebc6d521448ef6d033e1585a5ed6bcbcd1`  
		Last Modified: Tue, 02 Aug 2022 13:58:24 GMT  
		Size: 10.9 MB (10893408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a04cce4da471da7339c364869465ed016774874978f22acce2cc39bb9ead437`  
		Last Modified: Tue, 02 Aug 2022 13:58:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b65bdc45a558ffba287816e17e1126b9285c238098635aa3c00f6579301a3b2`  
		Last Modified: Tue, 02 Aug 2022 13:58:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c550336ebd94e7da67ecab9e9641d1125ae9892a6e53beb15510cdaeb177d7`  
		Last Modified: Tue, 02 Aug 2022 13:59:01 GMT  
		Size: 239.2 MB (239187767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d7f1bdf1bd7fd0f7d737e9250e43650de8b5e815bd77d8403f6834729f133c`  
		Last Modified: Tue, 02 Aug 2022 13:58:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf730b591358262d29294f063a2a095bb438b736d09b9867750da9a660388827`  
		Last Modified: Tue, 02 Aug 2022 13:59:22 GMT  
		Size: 86.6 MB (86568972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bafa8402824e8fc2746fac433d95ca63c18c25e7157347c220bb275e701214a`  
		Last Modified: Tue, 02 Aug 2022 13:59:09 GMT  
		Size: 317.8 KB (317845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c53a4a6a59b2d6fb99c5aa1d32fd18b873d7c25500236c513a2330680a399a`  
		Last Modified: Tue, 02 Aug 2022 13:59:20 GMT  
		Size: 76.0 MB (75976721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267ad0b82b0dbb9bb01d15864d86c5bc4a7f029b88bd6ff476a422cf665dba5`  
		Last Modified: Tue, 02 Aug 2022 14:01:06 GMT  
		Size: 488.0 MB (488014247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2e1d939d0d39d36d113dc6065fb0ae71f9207949f46f31e8a87a1cd7c51ea6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.7 MB (867664380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7a08645d17a3dda8e51a470fda30f3a96065c29cfdd1bec886137546446cf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:00:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:00:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jul 2022 13:00:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jul 2022 13:00:51 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 13:00:52 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jul 2022 13:00:53 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Jul 2022 13:02:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:02:13 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 12 Jul 2022 13:02:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jul 2022 13:02:16 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:02:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:02:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Jul 2022 13:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:06:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9d4034dfbab9d3d5107231bf79f7e9128aa4489cba93d97578d760166fe3e6`  
		Last Modified: Tue, 12 Jul 2022 13:09:17 GMT  
		Size: 10.7 MB (10689263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0120a667e47e68ebbd4a03de6b0932ea25a0078d49f8ee71a75c9ebc31fbeef`  
		Last Modified: Tue, 12 Jul 2022 13:09:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0820f1a42597e95311859510855953092a4ac35c4d590417693b084968c31`  
		Last Modified: Tue, 12 Jul 2022 13:09:16 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66081e680fda062b62d547ed9e29d0766f71a29d7a5fafb291a118efb1d184b`  
		Last Modified: Tue, 12 Jul 2022 13:09:46 GMT  
		Size: 184.4 MB (184372986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b195084a0c638927568ddb99e45b6b5b0c4d9994a11d7938842a8d3a60a9a1c`  
		Last Modified: Tue, 12 Jul 2022 13:09:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3d20692b99e02b1c6458a922737fcdd3c2672cdd5f388abec6574b69ba70a8`  
		Last Modified: Tue, 12 Jul 2022 13:10:06 GMT  
		Size: 84.4 MB (84370574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51c1b09402b429b070ef67b190db669048246a5a35cd21c29746c5765ab8eca`  
		Last Modified: Tue, 12 Jul 2022 13:09:55 GMT  
		Size: 316.4 KB (316388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02cb0af4b91439692d2e60c520d13a9ba0ab45163ac7803dc675c1d54006746`  
		Last Modified: Tue, 12 Jul 2022 13:10:05 GMT  
		Size: 73.9 MB (73865065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2296917a8ccce27517c4119004e34bdbeac749fe6693ee3f50568b941dc30b`  
		Last Modified: Tue, 12 Jul 2022 13:11:31 GMT  
		Size: 464.8 MB (464818808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
