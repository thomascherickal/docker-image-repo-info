## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:f648b7b579bbb8c266e06ac19eb1cb3bf282fd296b1c4fcab5325a3560614255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:98e2d4243495d98e5c9262e4df317d9f2a47d8c4768adbc67debed2aba8f429c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **828.6 MB (828590049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76da559adbfdcabc8fa56c54180dc823ecdbe658b27f555e294bed911400064a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:09:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:09:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 May 2021 17:09:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 May 2021 17:09:16 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 17:09:17 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 May 2021 17:09:17 GMT
ENV ROS_DISTRO=melodic
# Wed, 12 May 2021 17:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 12 May 2021 17:10:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 May 2021 17:10:50 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:11:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:11:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 May 2021 17:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:14:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a867e9d598a219f826e3b76f5280f3d106205d5fa6b8e1f2d421fd463d8fbc`  
		Last Modified: Wed, 12 May 2021 17:21:34 GMT  
		Size: 6.9 MB (6869206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302212f98ddaf07466a1b811fe425f01ff9f85b2778ce2d5b97611934d34240f`  
		Last Modified: Wed, 12 May 2021 17:21:33 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b35ff6673ef12169b553429937e2fe4a366a68e6eb03770829a0b95f3361ad`  
		Last Modified: Wed, 12 May 2021 17:21:34 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70bec3846c6a4887618d8cf19d2db025d8d2122df811164567153330bf2e1a8`  
		Last Modified: Wed, 12 May 2021 17:22:22 GMT  
		Size: 270.0 MB (270044121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0faf0f68b02c8fbcd34133d9f9b4bc1413a3f0851320b60e97d7f30e2404b931`  
		Last Modified: Wed, 12 May 2021 17:21:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5542020de522c68695172342481ec3eb28e50500ff526fa7af67c329da7b7b2b`  
		Last Modified: Wed, 12 May 2021 17:22:45 GMT  
		Size: 70.2 MB (70153767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6bff56dc550773ba81dc63cdc50b0a51f817a1c5d8a613db08f79e0484287`  
		Last Modified: Wed, 12 May 2021 17:22:32 GMT  
		Size: 264.0 KB (264024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cb4d3b0a8144bac01a9f75f0f783076bca2e1810e5651798155f967fd4ad95`  
		Last Modified: Wed, 12 May 2021 17:22:42 GMT  
		Size: 55.1 MB (55059368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45679ec7eb5a6bc0d2bdaea7f7f5d19a41ecc0d50f00d652e21474b1f809688e`  
		Last Modified: Wed, 12 May 2021 17:24:11 GMT  
		Size: 380.8 MB (380817664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ffc7568848eb94a2dd41069e653c3ecaa29a15c8def908a490ba0cb33ba87dc2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **749.8 MB (749819290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6dae97701efcf65ea191c22a61df2026a902eebf89988393c5f2a56dd673c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Thu, 27 May 2021 15:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:04:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 27 May 2021 15:04:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 27 May 2021 15:04:57 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 15:04:57 GMT
ENV LC_ALL=C.UTF-8
# Thu, 27 May 2021 15:04:57 GMT
ENV ROS_DISTRO=melodic
# Thu, 27 May 2021 15:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 27 May 2021 15:06:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 27 May 2021 15:06:15 GMT
CMD ["bash"]
# Thu, 27 May 2021 15:06:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 27 May 2021 15:07:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:09:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a98e1e3f21a423192b7c1a0497b1b7bfc382689c0aff9a0673c2497a89c2f9f`  
		Last Modified: Thu, 27 May 2021 15:40:04 GMT  
		Size: 6.4 MB (6442854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aec0a67d93178c66f703b46387890df2610467fc051d6d75bbeb69084cfe7f9`  
		Last Modified: Thu, 27 May 2021 15:40:04 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d81359b86841e869b88f3722c9d07b8bad9165ee109b14f0e019d09d7ec95f`  
		Last Modified: Thu, 27 May 2021 15:40:03 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481a6394104cb7b757467168f40d8aac2412a1c4e71b6a60767c0254f15746e`  
		Last Modified: Thu, 27 May 2021 15:40:50 GMT  
		Size: 225.1 MB (225116762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8a806cbdcc74413856d83aae37a9b56f48ce5d4acec963f8b78155d9565ab`  
		Last Modified: Thu, 27 May 2021 15:40:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b91766c8f4b20ea71f87691d24ca7e954a5021ffd644e367da405d4ad51bcb0`  
		Last Modified: Thu, 27 May 2021 15:41:10 GMT  
		Size: 64.8 MB (64848777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4d09dca7a29aa40d2f8b0f7516523d2099899a6a25a4a9975e38ffaa426d87`  
		Last Modified: Thu, 27 May 2021 15:40:59 GMT  
		Size: 265.8 KB (265822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eca3e966fe5812175151dbb0c55bdcc904a85b991e115a92c59d8e425211478`  
		Last Modified: Thu, 27 May 2021 15:41:09 GMT  
		Size: 53.2 MB (53241751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5396c63de8d155958a56d464b9c5421556ad34305235153badd5185c038974e6`  
		Last Modified: Thu, 27 May 2021 15:42:38 GMT  
		Size: 356.7 MB (356723685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
