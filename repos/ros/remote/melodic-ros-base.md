## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:d8ecfbf20c635571e83e8377718eeab85ee581e118a3cdec8be8e078810106ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:fb723744019f7fd23ecdf827d98f438840ed49bc04be33b84b9394c90c2c20cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437545037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3373bdb88182d13d88b174fec2db62c13515f5c07f9e9f99accde09d5e431d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:16:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:16:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:16:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 19:20:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:20:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:20:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:20:44 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:21:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:21:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2dc1af9e78c8c03b3784e97b0c62313c5c52add693cb706e068fcce901459`  
		Last Modified: Tue, 31 Jan 2023 20:06:29 GMT  
		Size: 4.9 MB (4878622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ce8ecd18ce9a61cc5b737d625584f81283c15635bf0c0f055c4c0b3a67563`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71cc8d37cc871d60eee81184bc6d8a1e1c866501778e161631792888554553`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bb8fdfb699e9ced52d11673eb22698de7487b7fc88a857f4508b0a950e9c01`  
		Last Modified: Tue, 31 Jan 2023 20:07:02 GMT  
		Size: 259.6 MB (259570609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1291bf00d97c79825103e22492524225aeab5e47bbd31ab04844639b765db48`  
		Last Modified: Tue, 31 Jan 2023 20:06:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d4df0a9d6cae5901fa83c22b170c6613ec8554355268edd38fa9474b59df15`  
		Last Modified: Tue, 31 Jan 2023 20:07:21 GMT  
		Size: 70.3 MB (70266400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe392d68e0b6456c752bccd1fb9cf78e14ab1a3e5e740974f70f35496e719dda`  
		Last Modified: Tue, 31 Jan 2023 20:07:11 GMT  
		Size: 296.5 KB (296510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023408b2b9e07a73bca7c237d1219b5bcc04e13cc52633064f49e90fe444019e`  
		Last Modified: Tue, 31 Jan 2023 20:07:23 GMT  
		Size: 75.0 MB (75000498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:c2bb574e034735f687dad3f78b30822b56f93ecc67099939469a79b8732190ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62a82935fb270cc1459cc69df1e3ffba90f30fd177f408c00150af724fa04b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:20:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:20:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 18:20:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 18:20:23 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Jan 2023 18:23:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 18:23:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 18:23:41 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 18:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 18:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec3bd771f252293c5a70a0e50b16a27aa4cc182d5d5c4944c803b38ad12da038`  
		Last Modified: Tue, 31 Jan 2023 18:14:25 GMT  
		Size: 22.3 MB (22306068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bc29158f865556f2328416deec408f89e4d5a959fac7ce4e350e350cf9948`  
		Last Modified: Tue, 31 Jan 2023 18:48:36 GMT  
		Size: 819.9 KB (819866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3252175da0105a82655f398b29438a19ec2e04f09ab235f83c29a401118f52df`  
		Last Modified: Tue, 31 Jan 2023 18:48:35 GMT  
		Size: 4.1 MB (4090515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a38036063f67ca8d81ea7a7c48a0913f990ecc729a0f15ee4f76c8a1357c5`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e5eb71797c26c4e2ace97586f0a68a43ce039f27828c6cf21272575ed2e6d7`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857a22c653cbfa30c01daeec86e851722e951de12cf98b755879a24931968d2`  
		Last Modified: Tue, 31 Jan 2023 18:49:15 GMT  
		Size: 239.0 MB (239028794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1278f26ed1cb273ce9811a04653bd478c9ef002fe208fbd3e55bc3c453d0f08b`  
		Last Modified: Tue, 31 Jan 2023 18:48:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aeaf0eee0ac2d0004bc039c468a9230185faf6a37bf6d59d066a08d4500d90`  
		Last Modified: Tue, 31 Jan 2023 18:49:34 GMT  
		Size: 54.7 MB (54734814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae25993c4669492bc1aa92d06f588563bc78055f50aaadd125d0f334dd5299`  
		Last Modified: Tue, 31 Jan 2023 18:49:26 GMT  
		Size: 296.5 KB (296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7420fb008761a5a6d4974897a05891dd41de92eb360067fd91f6756bb177634`  
		Last Modified: Tue, 31 Jan 2023 18:49:38 GMT  
		Size: 64.8 MB (64750001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e270a7432c93f738fb6cb42ae04726c84dee53c855f2cb43c9fae71d373a7a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412192920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afc8882704f4a7b5cd865f8bffa9416bc6ddb23ffdf7cbf0d0a81e4be623b99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
