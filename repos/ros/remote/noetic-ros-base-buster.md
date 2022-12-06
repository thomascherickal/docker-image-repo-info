## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:2e40b1aa0f835c79808578debb495379c7875608c10f75a1c8b3318f25e58eb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:557c3ff19363df95f285ddae1bf9c1aba8d995cff0d3b09af2c22d6440a1e443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463448725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22d88eb290785db32ee5251e5d53b94649df5b88c1c68c82ee87a233aa965f89`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 06:55:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:55:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 06 Dec 2022 06:55:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 06 Dec 2022 06:55:41 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 06:55:41 GMT
ENV LC_ALL=C.UTF-8
# Tue, 06 Dec 2022 06:55:41 GMT
ENV ROS_DISTRO=noetic
# Tue, 06 Dec 2022 06:57:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:57:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 06 Dec 2022 06:57:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 06 Dec 2022 06:57:15 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 06:57:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:57:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 06 Dec 2022 06:58:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821976fb70a1a949ce1e0f957ab373f10caff567977865f6e32aa1c8e0f0aa67`  
		Last Modified: Tue, 06 Dec 2022 07:03:56 GMT  
		Size: 10.9 MB (10896976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a368d393abce7be1308b98ad183e4e4e4b0ceab2dc5e6d66a4f270e3b60209`  
		Last Modified: Tue, 06 Dec 2022 07:03:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e639599375ee6d0b5e7ec7f657f4e583e08f7647519f83dd8816c2a514666d`  
		Last Modified: Tue, 06 Dec 2022 07:03:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27796b9579d3ee5904e92b8b0d48179d0f2079d8bda295f20ba361c7245a6fa`  
		Last Modified: Tue, 06 Dec 2022 07:04:27 GMT  
		Size: 239.2 MB (239202286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c9359756e3a8a665915f05eb2303d5b7cb66ee058e2ff79826c06765230dad`  
		Last Modified: Tue, 06 Dec 2022 07:03:54 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fd814dd0b5bda31d27396eaf2509afd8e7c8790c37db6d900d21fb7ff39158`  
		Last Modified: Tue, 06 Dec 2022 07:04:45 GMT  
		Size: 86.6 MB (86585374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05ba9ebd536d110dcb0deb3f0a37fa8deab9e1e8eebdf80f97d62de5e35fb9b`  
		Last Modified: Tue, 06 Dec 2022 07:04:33 GMT  
		Size: 334.6 KB (334635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977ca706cab98b86bcd6627819d410bccfc7a94d7e81418011f198524bd5548f`  
		Last Modified: Tue, 06 Dec 2022 07:04:43 GMT  
		Size: 76.0 MB (75978177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fb6e515e06a57a82bb2063098c64f6fe96ba20bd81884c8ed02e4108d7623986
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403324372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5306cc2e39de31be333a308e132c2479a57efa54894ffbeaa9fa1ff334ee8001`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:24 GMT
ADD file:2deba7c04e28d01997b865f366cdc8d38a80aa39720c4e4d1fc581ac17e8ce4a in / 
# Tue, 06 Dec 2022 01:40:25 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:43:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:43:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 06 Dec 2022 12:43:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 06 Dec 2022 12:43:22 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 12:43:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 06 Dec 2022 12:43:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 06 Dec 2022 12:44:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:44:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 06 Dec 2022 12:44:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 06 Dec 2022 12:44:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:45:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:45:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 06 Dec 2022 12:46:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d0ec2abdb05569eada58143acd16d47ee4b07a33535544cf5bf267bde20cc3`  
		Last Modified: Tue, 06 Dec 2022 01:44:13 GMT  
		Size: 49.2 MB (49233737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19909c3aceadf49713a2958f24157589411bbf1dcc27234877c791533c4931cc`  
		Last Modified: Tue, 06 Dec 2022 12:52:31 GMT  
		Size: 10.9 MB (10902551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0181cf3cb0b9040387832394cc9847f4177ae05dac529dfacddb2f2312f1a`  
		Last Modified: Tue, 06 Dec 2022 12:52:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eb2f304753cc8ea4ffdbc3773c8b3f7a6cc92f42e9e2b457f18c686b552e0c`  
		Last Modified: Tue, 06 Dec 2022 12:52:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c9f6486d36ebb5f36eeef07be3a7f5e666f02fe29bed9e356f9b3f28a0ac03`  
		Last Modified: Tue, 06 Dec 2022 12:52:53 GMT  
		Size: 184.4 MB (184389225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08199b0f516be12421278daf2cfe3f49eadd36aa15280052a1e3f9150f604050`  
		Last Modified: Tue, 06 Dec 2022 12:52:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90588e293a56d63db24ea1d7234cbda9a4d93b1aa5e84fc3a75eca2a74c263f`  
		Last Modified: Tue, 06 Dec 2022 12:53:07 GMT  
		Size: 84.4 MB (84372220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92efafcac5386f96dc9e4608ed0600788f384d32ec0fdeefb55d00449fea4051`  
		Last Modified: Tue, 06 Dec 2022 12:52:58 GMT  
		Size: 334.6 KB (334637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132edaeef7af72f03ca08f244b2d01dda26540f3d1f0135a92535a575b1752ac`  
		Last Modified: Tue, 06 Dec 2022 12:53:06 GMT  
		Size: 74.1 MB (74089588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
