## `ros:melodic-perception`

```console
$ docker pull ros@sha256:f55331133cf06ca467dc5cc6f5b5451dd07f8c4e8814b60f56c67e9d83c4700b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:40cfa4e6831580a7e94f926d9f613b895e3b52f952cbcdc219e9485241e96727
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742495840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c120ce65b173ba9ad84e2093d1cafe125e619fb43feab4675476c57d1c7a67f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:23:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:23:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:23:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:23:07 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:23:07 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:23:08 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 04:27:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:27:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:27:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:27:19 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:28:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:28:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cd3aa01fa8a2dad33dee176be919cf9e72b3b56c4289e1c823911634874027`  
		Last Modified: Tue, 31 Aug 2021 05:00:05 GMT  
		Size: 840.6 KB (840612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99886d4d51f082d03e74f007db2abfbb1d29194e23d5d765bc290cf61fbf9f62`  
		Last Modified: Tue, 31 Aug 2021 05:00:04 GMT  
		Size: 4.9 MB (4872181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f194285c94f6dea3979938b6fbee0d4a2d6519963cd65e91529bef9bacb761d5`  
		Last Modified: Tue, 31 Aug 2021 05:00:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1c58b68bff83012aef442563da9d5134c789059e41afdfee20487a62ecc11e`  
		Last Modified: Tue, 31 Aug 2021 05:00:02 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc52136acd257c37f9da7ccf4926aaa20dce788c25653e41cb17f2a893217265`  
		Last Modified: Tue, 31 Aug 2021 05:00:44 GMT  
		Size: 259.5 MB (259453751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b39e205d1502b2e7d3b1063c045c77be339ed5b2be5d436f6ac94938787fb9`  
		Last Modified: Tue, 31 Aug 2021 05:00:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d962448be0992e4d09cbc08ceb5257e02d7f27d7a162bd2ca47201ea525f6a8`  
		Last Modified: Tue, 31 Aug 2021 05:01:06 GMT  
		Size: 70.2 MB (70229946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd15864b223671d593d514c379a0466ebe41350c6c094fd51dfdc708eeaf0ca`  
		Last Modified: Tue, 31 Aug 2021 05:00:55 GMT  
		Size: 271.6 KB (271586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfbc4d61cac2ce2df5fe609fdd06c25081bd30deae2b98209d703fa99b75cc9`  
		Last Modified: Tue, 31 Aug 2021 05:01:08 GMT  
		Size: 75.0 MB (74994320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ade1654cf3837b22a2f51dfb4b700089179cbb01b73ccabc8be402baf4a40`  
		Last Modified: Tue, 31 Aug 2021 05:02:25 GMT  
		Size: 305.1 MB (305122516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:0d0b271cefece9d849742e548b1afcd6fbec30fd01d71a41b2469ffe80c0d3ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645755710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:475371a853eaad75e2747a0825878fb9487b24decd736155c7bfe08c830b60b0`
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
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c6e087ef5b3f497715fda3ccbc7df571758e90ab212c4db508d80873296f37`  
		Last Modified: Tue, 31 Aug 2021 04:17:13 GMT  
		Size: 259.9 MB (259877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:90cbdcadb40a69fb9c9af3076c43913647e0decfabab70796c571b35fea4fd15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703413809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b8dff296c7ff902c567db32969e245f3f6c73814572a8512817fdb32991f3b`
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
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c42f2f049dbe2df2b2e9101fd5b273df3b006c906cc94a31e261a4802b5e060`  
		Last Modified: Fri, 01 Oct 2021 04:21:00 GMT  
		Size: 291.5 MB (291464530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
