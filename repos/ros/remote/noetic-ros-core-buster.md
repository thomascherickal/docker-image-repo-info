## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:b3a823a1c4c4c043e01f54a2396ff4c7dfc5f8cfed9dc47794f4254bd0812b13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:2c50e8c3d36e29203b9f3c0f5cc5937b65702932c7af75b46e3297ea653c4e7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300550539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8233aa7bd2facad013538e003fdd08eb0c1e5ac30e030b2e519dc8c56858ce8c`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13b6153477157fac96d5d4bd40b2d2d50c8c6af78592c40f9b730f82585f83da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244527927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ad9762e737d4f4a55ab2dac10bc03e5a40b4769db05bc655472c1727e49973a`
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
