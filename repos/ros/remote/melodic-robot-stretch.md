## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:06374cafd79e4aa9858181916f1ae3044abf8a4960c6f98049208e3f7ea5cc23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:9eab8f485527e73c6acf41c942c14c6dc3dfee5d6b324efadd87c2e425ef4b9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **462.7 MB (462665674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc2a15be60c5d8a383ee6143a77784106e146d34eeda983ee61734dbb8e51a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:29:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:29:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 22 Jul 2020 20:29:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 22 Jul 2020 20:29:42 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 20:29:42 GMT
ENV LC_ALL=C.UTF-8
# Wed, 22 Jul 2020 20:29:42 GMT
ENV ROS_DISTRO=melodic
# Wed, 22 Jul 2020 20:31:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:31:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 22 Jul 2020 20:31:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 22 Jul 2020 20:31:36 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:32:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:32:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 22 Jul 2020 20:33:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:33:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40906fc9f8b2b8a56bcfb4722f5852e4b44c411ca4920de277f8918bda8cf4f`  
		Last Modified: Wed, 22 Jul 2020 20:45:35 GMT  
		Size: 6.9 MB (6866450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d372ce5eef2222822237de281a86ffbf352f436e4a2d0c8c6004bff4b1bab`  
		Last Modified: Wed, 22 Jul 2020 20:45:34 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18fe21b5c4a5260fb018eb41aeea35891bd8c794ac4577cc34bdf43e09d0fe3`  
		Last Modified: Wed, 22 Jul 2020 20:45:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78d712f176959e0679792cfa27f71e34bab75b51798bcc66a97b4895e3c656e`  
		Last Modified: Wed, 22 Jul 2020 20:46:52 GMT  
		Size: 269.9 MB (269880803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c160d001a2a5b6a00b738e8015b92469234b60e6f5dfbecf7b4aa4699b0590be`  
		Last Modified: Wed, 22 Jul 2020 20:45:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17e9bc7f05fd42e803d8842676c9843e8fdfdc3ad163a1725dbe58fbe832a5d`  
		Last Modified: Wed, 22 Jul 2020 20:47:18 GMT  
		Size: 70.1 MB (70149773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321b75213e5c39b58eb62ac16279838200f9ae2a58fd1fb7cf79ed08c441fc`  
		Last Modified: Wed, 22 Jul 2020 20:46:56 GMT  
		Size: 254.0 KB (253982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac773c927ecffa716e5d95666c65c78f2eaf4b8010c7cd52ca68c2dcb98860a`  
		Last Modified: Wed, 22 Jul 2020 20:47:17 GMT  
		Size: 55.1 MB (55051919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea68892efe9ed6d67e1beec6d690804cd75756b841cb39f4b71c2b1ee9f008f8`  
		Last Modified: Wed, 22 Jul 2020 20:47:27 GMT  
		Size: 15.1 MB (15091257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4311178ae18c8a9366f0f0460f4e0591c3ea99662cce90939a4ba3d107bfe04
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.5 MB (407516405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8de25d1a9f5b0b61417d250572aa55c27919115720c03354da00cc4623a87913`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:42 GMT
ADD file:9c5c9df9952cb51291333837bdb462bbdf9f157e91e616f1e3fb8d2fcb1a1983 in / 
# Wed, 22 Jul 2020 00:43:45 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:25:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:25:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 22 Jul 2020 19:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 22 Jul 2020 19:26:10 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 19:26:14 GMT
ENV LC_ALL=C.UTF-8
# Wed, 22 Jul 2020 19:26:16 GMT
ENV ROS_DISTRO=melodic
# Wed, 22 Jul 2020 19:30:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:30:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 22 Jul 2020 19:30:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 22 Jul 2020 19:30:23 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:31:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:31:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 22 Jul 2020 19:33:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:34:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad4de4f68e9c2c0f5e5e62d379d936bb88ce467505ed002fb1e10c434fefe90c`  
		Last Modified: Wed, 22 Jul 2020 00:49:52 GMT  
		Size: 43.2 MB (43169407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585176f5de99b8e33359e78fe9cd34f20da6cf5724e665a8f2298c4e08a2c01f`  
		Last Modified: Wed, 22 Jul 2020 19:58:33 GMT  
		Size: 6.4 MB (6438780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03065d637722b646c143464a227682878b2e718150a24a8330bf249ea91391ef`  
		Last Modified: Wed, 22 Jul 2020 19:58:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682b45741119383dec6695aefd378294f6b562056f0339f1f1955db84f2001e0`  
		Last Modified: Wed, 22 Jul 2020 19:58:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a464bacf6f2264fb00064f902ee0a88ab0809f727acda3fa174eee7c97595e`  
		Last Modified: Wed, 22 Jul 2020 19:59:57 GMT  
		Size: 225.0 MB (224953934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2acfe8e8d7f95c79bbcb21d3a9f931ee58d52bee040afac16b87be02b940003`  
		Last Modified: Wed, 22 Jul 2020 19:58:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243df2136f331d3be62549924b6e4bb6b48cef2919e840054c5b8a810cb0ba1e`  
		Last Modified: Wed, 22 Jul 2020 20:00:24 GMT  
		Size: 64.8 MB (64836222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c43b3fca6d5121261cd09c44c321c34a02208fae74092b1690d18ef9694cc`  
		Last Modified: Wed, 22 Jul 2020 20:00:04 GMT  
		Size: 253.8 KB (253849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a76dc9ae5004d0aff32a490571832256bb63fcb072c618b7a7a3a1fc72025b8`  
		Last Modified: Wed, 22 Jul 2020 20:00:23 GMT  
		Size: 53.2 MB (53222677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12826b5fb76b24765d79720be2b4265bec17de78e25b35c45706dd7209fa28be`  
		Last Modified: Wed, 22 Jul 2020 20:00:34 GMT  
		Size: 14.6 MB (14639718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
