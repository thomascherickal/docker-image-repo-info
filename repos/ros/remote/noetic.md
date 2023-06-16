## `ros:noetic`

```console
$ docker pull ros@sha256:354822afe7a245df758e5a8486a079674495a5a9112eb2e599f9b8f5dd5ffd9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:f10dcf5c7de2ebdf90dc2fe1c0c17359ad44d184c307c37945dbf6868c74c1bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d932427105199181dca9d9ad90a855f7e395ad62ca98042928922c4b4c833dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:00362f93138beaccc2f24ca7603855ad9e5c4c1d0fb3276731ec5cd2c9e1a194
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289312397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb397f715f738fabd09fe73d93f3af1988aebe53ecd1c2e419665dd65abef97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d5ea21ddeb3a8263b55ff73a81ba0a53954362e89dbb5bc3070f7c55b5e8c6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322836771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc8c46b2872805b8ba64f84218bf3b7ff59ec0c72e34a2e11a8be1df5048b440`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
