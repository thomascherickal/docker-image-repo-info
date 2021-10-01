## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:b0f161182c43d7ac34e4db52559119570e0e4b20fd867463979a2fdc561ccc3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5da99077487fb6a23334589c87442544965eff9960b0aef3bb5b385f60d6264a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291875817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ddab15692c93b05ddb281246caa09b9c5d97794a953a331cf7a991ee9f7e8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3f037fed4337561cafeeeb154ff906161749d68f484f3fa0151c0e7edbee788
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266165014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e07be8dccd80381c769ac0d786fcf34a2755ea28b9a33678ff833e22c090e9f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2bc12f70d7412f29e9c8c5a6233b3024c9b95127c8eb57972f310761565fca27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281394523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9583134313a6bba2702d7dd1d42064e6609ff036c2e1a61bf2a50b9b322300ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
