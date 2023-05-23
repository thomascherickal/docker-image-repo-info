## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:f6aee5d0747b13580ce2f8f044fdd75095607ee055e8bdab64b99c4522473ad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:b1db5de3c20d2e22ead61a7bf5d3c7a2e0bd17c3a51dfb3ad5e79abb064237e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484664045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e7c8b36b79c9686088bb1bb19f60151e21b53fd8dd31676eb5537c06fe5071`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:38:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:38:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 21:38:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:38:39 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 21:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:39:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 21:39:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:40:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:40:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:40:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:41:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a520b96cab6be544c3de79dfbd2e79a43648778ff5ffc9cea03b9afea1a8a`  
		Last Modified: Wed, 03 May 2023 22:02:33 GMT  
		Size: 10.9 MB (10897025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b18fd569bd474fa851fd78f1d3bf2e9678d8423061fdd217c621a34a0e1a18`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b96262d8a19c986620307e5e5f5bc87d241ebddd343a22e317096193e83ca7`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba9b33e9316a950f2ca0db084e17331cca39064c3a3d10175a5732482915e1c`  
		Last Modified: Wed, 03 May 2023 22:03:02 GMT  
		Size: 239.3 MB (239262397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f679b704b1a974ebf77923991309e3935a8e4e5950043f8e8df9817cb566018`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0114f4c6a2082f6e76098833ebdf4262123ac4a571969bf9e9e38f3b7160e730`  
		Last Modified: Wed, 03 May 2023 22:03:20 GMT  
		Size: 86.6 MB (86625207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1570d96e90fa78b5cc55358c3d0cce3f912d1c9ce9118a0c94901ba67a8a2ab`  
		Last Modified: Wed, 03 May 2023 22:03:09 GMT  
		Size: 293.2 KB (293249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f61e4fbe9210080b697fa8cf61250a48a94b4b6784227406fff9b625ad3878`  
		Last Modified: Wed, 03 May 2023 22:03:18 GMT  
		Size: 76.0 MB (75978108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970cf90ffb56b90e32ca3b5e62c8d081c47000f6ef2addf1ff37158692e7438c`  
		Last Modified: Wed, 03 May 2023 22:03:28 GMT  
		Size: 21.2 MB (21156951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:50bb12073608fc106b929a22e72e30d3ffa649fab34d075bb37895a9b25dd406
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424196844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3e7980c8f20e0b28634d551d75871da9017c1421a0d3a4fe5bb53f69112944`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:21 GMT
ADD file:a5100e7ed3c2665c1b4dfbb32eb2b47b85783f2a6800e0ae9004db0ce021dfa5 in / 
# Tue, 23 May 2023 00:43:22 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:09:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:09:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 May 2023 07:09:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 May 2023 07:09:55 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 07:09:55 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 May 2023 07:09:55 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 May 2023 07:11:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:11:26 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 May 2023 07:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 May 2023 07:11:26 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:11:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:12:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 May 2023 07:13:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:13:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ea482247e9a0d1ae4ed218fb0828063b9cce53822e64fd4621f587ab85a7e6d`  
		Last Modified: Tue, 23 May 2023 00:46:24 GMT  
		Size: 49.2 MB (49238292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62aacc6d8d227c977953e480d4a68a0de585d973ccb199b674eb74cfae11ac6`  
		Last Modified: Tue, 23 May 2023 07:18:45 GMT  
		Size: 10.9 MB (10902726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44af36709d88eec5e6f50342c165ae44b26b6b1697b4445ad71fcde5bb66f72d`  
		Last Modified: Tue, 23 May 2023 07:18:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf23de21b4a8076854c4b81c2da993b3eb5504eb2993919efc62d70f024cc8f`  
		Last Modified: Tue, 23 May 2023 07:18:44 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e704756b8ca302bb92f857a7f79fa9bbe4245d11fd39fa2b48ad558d5ce859c`  
		Last Modified: Tue, 23 May 2023 07:19:05 GMT  
		Size: 184.5 MB (184450768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5cdc9acd26d4497666808bec531405faf0715bad80e7d3c9b4e865a8d80609`  
		Last Modified: Tue, 23 May 2023 07:18:44 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e339807dcdea4df15d2c46a5d429937129828e8742a63c58e7e9cd6b79a5f209`  
		Last Modified: Tue, 23 May 2023 07:19:19 GMT  
		Size: 84.4 MB (84397050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8edf64563834cf13dd87b16e82ca48379a6c011de4f3d8240641dca72fb457`  
		Last Modified: Tue, 23 May 2023 07:19:12 GMT  
		Size: 293.6 KB (293598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8cbf35aa60a417abbe378d7ee172e069be9971caa123cc79f0999f8b248137`  
		Last Modified: Tue, 23 May 2023 07:19:19 GMT  
		Size: 74.1 MB (74090723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70618ae76a4d3e2c4d8d6217d970d9d4c457e88342c0b3601cc0fe71cfe514ef`  
		Last Modified: Tue, 23 May 2023 07:19:28 GMT  
		Size: 20.8 MB (20821276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
