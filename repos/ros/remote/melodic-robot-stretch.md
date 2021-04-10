## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:1f49f27092b981e2049a387fc217ca832afb8b018eb8256d8e154179501b89ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:f6776ca30f410dcd5b4ae2aa41e67a5d9fce8282085cecfabf66067afa6725a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **462.9 MB (462886128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4439997410dd6d9e0755f7dd8424f1dc6c471dc50ef5b903f90d6bba15a1927`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:23:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:23:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 10 Apr 2021 17:23:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 10 Apr 2021 17:23:30 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 17:23:30 GMT
ENV LC_ALL=C.UTF-8
# Sat, 10 Apr 2021 17:23:30 GMT
ENV ROS_DISTRO=melodic
# Sat, 10 Apr 2021 17:24:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:24:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 10 Apr 2021 17:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 10 Apr 2021 17:24:53 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:25:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 10 Apr 2021 17:25:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:26:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b6b37ff3c9e7747e5ebcec4e9653664f6b4d5aae65d0ca6426f96d150b07ef`  
		Last Modified: Sat, 10 Apr 2021 17:36:26 GMT  
		Size: 6.9 MB (6869236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed11cf2e4670457c8f93ec97baa3961a99e6a2d658098e2543d69327824907ba`  
		Last Modified: Sat, 10 Apr 2021 17:36:25 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaa2ec57725ac5d6cbd09c1a38d501aa47f8619fbea04756c27c89000efae76`  
		Last Modified: Sat, 10 Apr 2021 17:36:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79b4d54d6aefe904230029947ce2a9d6fea994fac3c29dbe525ea6c86dc9d3`  
		Last Modified: Sat, 10 Apr 2021 17:37:12 GMT  
		Size: 270.0 MB (270045795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d30700ac077f617ab3ad6e914e76bd7c148394ffafc97cefabad13cdbff9c34`  
		Last Modified: Sat, 10 Apr 2021 17:36:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d6df4fd34701663c0ed79ec68142383f08732c14ee74f1bcbf629f5c56b1d7`  
		Last Modified: Sat, 10 Apr 2021 17:37:34 GMT  
		Size: 70.2 MB (70152404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57814eec8f3ba718d413538f18411d2ec5a96b842bfd93e3ad4e83f7d09b3524`  
		Last Modified: Sat, 10 Apr 2021 17:37:21 GMT  
		Size: 251.5 KB (251515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a43f74306074df39eae3cadaa4aec3923cbafb2c057616c514b5b3cbc60b176`  
		Last Modified: Sat, 10 Apr 2021 17:37:30 GMT  
		Size: 55.1 MB (55058959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82515373f3c5d35cf7d4ae9aac313e227558bdbef9a8831e5f22e99fa11d1ceb`  
		Last Modified: Sat, 10 Apr 2021 17:37:45 GMT  
		Size: 15.1 MB (15126365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0f828873bd321b8e2a6dbbedd7cd13787f371ba667e94917b3b614bf9cff53ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.7 MB (407743712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6c6d056b315d1d888517c1b9ff27bc2a1f10562933ccc4f7cc976cbe12e91e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:24:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:25:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 10 Apr 2021 15:25:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 10 Apr 2021 15:25:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:25:11 GMT
ENV LC_ALL=C.UTF-8
# Sat, 10 Apr 2021 15:25:13 GMT
ENV ROS_DISTRO=melodic
# Sat, 10 Apr 2021 15:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:28:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 10 Apr 2021 15:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 10 Apr 2021 15:28:29 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 10 Apr 2021 15:30:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:31:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d267bb40382f265c3a2b17a40e3b0ac14aefec3241d3165a352fb9e8b3a3611`  
		Last Modified: Sat, 10 Apr 2021 15:51:31 GMT  
		Size: 6.4 MB (6442907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f409406543418e427fce300b8eb166b61fa11defc2b68267d6ffa9a507c77309`  
		Last Modified: Sat, 10 Apr 2021 15:51:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34172e3929e56eb4fba600b5c480baf8112d57abe120790cbe1befa7d3fb9e61`  
		Last Modified: Sat, 10 Apr 2021 15:51:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60954ec9568f6a7e2dbdddb363be902d336e96653dc84225e0e1fb5ba980ab66`  
		Last Modified: Sat, 10 Apr 2021 15:53:14 GMT  
		Size: 225.1 MB (225108617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95e19ab692b33c8148268009f1a7533000eb4b4c804fcdd8ce42321edce7d35`  
		Last Modified: Sat, 10 Apr 2021 15:51:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665759b1c2ca319d3fbc7fd1d3f169931874b128cd4fa7598871653363c2c545`  
		Last Modified: Sat, 10 Apr 2021 15:53:49 GMT  
		Size: 64.8 MB (64841566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa262508378f63ea709dfb9521e70536cb0fab5bf5d3e78bc5db723ef6978c9`  
		Last Modified: Sat, 10 Apr 2021 15:53:25 GMT  
		Size: 251.5 KB (251511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f21cf4fb5904d41f84d88f936971f252ee4c968e4f87fc4259658884064e1`  
		Last Modified: Sat, 10 Apr 2021 15:53:53 GMT  
		Size: 53.2 MB (53246575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648f8269f77d5b8529f3ac2ffd3bf83af69046337c65e6d598a46cea428d356c`  
		Last Modified: Sat, 10 Apr 2021 15:54:04 GMT  
		Size: 14.7 MB (14672946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
