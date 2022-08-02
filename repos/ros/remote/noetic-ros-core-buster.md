## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:76e2bd296a56dafc9785c0085b2bdd01dd4777183fb4cbdf5dd0cbd8e7500f1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:670d0f8f29324f5d15fe53c99f4cb268133580585924b92428ead3dc0dfb429e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300524569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a45164c156c820452f2bc1aa5c01e542e53f15a8349fa258fd4ee1197c5e1b`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:84f96828f39aee595f8614d70466b274a0ed49dab231f8804b068ede598aa4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244293545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:debf14ac309c743939181156899aa2cfbec1a71008241693dca29b060dd1a6ad`
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
