## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:91d3cb575dd45b80aeb0b5e23c70f87cd87368cd30d915775e012f12046f38a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:a7b68862f6510dc5da37cfe56e6f27b998df31385e5aaca93494c7cc84feaa64
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322296885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ce3724f9b38e9a5dec77794632a7e0760415a23429065d2399c9bad44be501`
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

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9c7656aec543122a885e3d585794c287601f79d360f3f34e77d680b192863e33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274731114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba461b1c7182bc79602fe5b404b31bd2d5eaeef9f296314848f097008318ad1d`
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
