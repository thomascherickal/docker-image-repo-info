## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:2ab384144555cfe256eea3339f71428adfb9abb9de053309a36407a1dc8ebf44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:19c2fba72ffb0619e06f01c79b0a119b098b8d0c5fd2010d243f3c9b5cb31f90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **462.8 MB (462820948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a284b97874fee349dfcd0a1829649b6bc54995bc27afa0e64a76c324d56fb89`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:24:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:24:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 11:24:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 11:24:15 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 11:24:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 11:24:16 GMT
ENV ROS_DISTRO=melodic
# Tue, 09 Feb 2021 11:26:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:26:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 11:26:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 11:26:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:26:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:27:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Feb 2021 11:27:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:28:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfef8404fefc17dca87eada52dd07e7bf488497c0c31fea11a60d978da694ad`  
		Last Modified: Tue, 09 Feb 2021 11:41:05 GMT  
		Size: 6.9 MB (6868182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6e767fccda9923a28109011a5e7fdda7e9f5841c99cc59bee58d437744ceaa`  
		Last Modified: Tue, 09 Feb 2021 11:41:03 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973024f9f826542d72aca896bca3ed1f99093289ca8442460a1d25549bed8bcd`  
		Last Modified: Tue, 09 Feb 2021 11:41:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a0b85ea3938d10333f243bfd23c5bed7f06b58b3a5aaaeca4007a5e2b2eb84`  
		Last Modified: Tue, 09 Feb 2021 11:42:10 GMT  
		Size: 270.0 MB (269998323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36fe789310fd477065fed5386f3d7ac24047a56072617d59131f960a643d88`  
		Last Modified: Tue, 09 Feb 2021 11:41:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74144c81a256f811ce993305c224a0dbe9432e6de9707d6362cc46160e2a20`  
		Last Modified: Tue, 09 Feb 2021 11:42:51 GMT  
		Size: 70.2 MB (70152536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db447f03061cc7b020dab71976df77709f2668c750794810919c0d7494d6d3`  
		Last Modified: Tue, 09 Feb 2021 11:42:15 GMT  
		Size: 246.4 KB (246447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca203fed66a213b3b04ebec6a1c62c6c7ee68c202941aa3289672514f40906c7`  
		Last Modified: Tue, 09 Feb 2021 11:42:39 GMT  
		Size: 55.1 MB (55053684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00874da3b581cb842ffaa7176113afe392e05c93005342bb55a1d357463ff02`  
		Last Modified: Tue, 09 Feb 2021 11:43:01 GMT  
		Size: 15.1 MB (15120075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d9e7242ebafd7757ec25d4e69b253e26318ee3191009da8a681ffb8924cc0aff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.7 MB (407718544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daae786157207966b368bf3936cc1bb29df89cfb39c8f49e4b6207daef0e02c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:52:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:52:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jan 2021 16:52:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jan 2021 16:52:58 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 16:52:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jan 2021 16:52:59 GMT
ENV ROS_DISTRO=melodic
# Tue, 12 Jan 2021 16:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:55:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Jan 2021 16:55:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jan 2021 16:55:44 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:56:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:56:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Jan 2021 16:57:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e8239a7d8ab4bee604fb1cbe80d3b4626bc8acc2aac57b72c796f1df90dcfc`  
		Last Modified: Tue, 12 Jan 2021 17:19:42 GMT  
		Size: 6.4 MB (6442128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba0c86565e756ed3e4b30d4defdb5a05c4fa9003af196a2339f78ee34d7327a`  
		Last Modified: Tue, 12 Jan 2021 17:19:41 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1b375834829a4e5e0a592407ed74f1602a3d9b06b46e344684c89d9cb32f29`  
		Last Modified: Tue, 12 Jan 2021 17:19:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41b4520c9fa74d7df36a1d382749cb9a1cc38894d750c425a64ba26e1ab86f3`  
		Last Modified: Tue, 12 Jan 2021 17:20:40 GMT  
		Size: 225.1 MB (225095855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7f1a09c11b17890907dd9234634ee66ce853062cc262bc85d6fa2eff682c80`  
		Last Modified: Tue, 12 Jan 2021 17:19:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e007e9fd419b94a9e3973bea456a0488bc87d4896cc50f48d151eb90c501db2`  
		Last Modified: Tue, 12 Jan 2021 17:21:10 GMT  
		Size: 64.8 MB (64841363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5996f090d2e43890c4b004ee289bcf1368c596deaeaa867d237956c1fed69943`  
		Last Modified: Tue, 12 Jan 2021 17:20:49 GMT  
		Size: 243.9 KB (243873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebac23cb600e01b4ad85eb361f8a14d22b24401d3db4cb7b416134632a67eafb`  
		Last Modified: Tue, 12 Jan 2021 17:21:03 GMT  
		Size: 53.2 MB (53242822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32ffc9f464b01e8b02e4f1c0975973d4df55fba17633d734231dac06dc85256`  
		Last Modified: Tue, 12 Jan 2021 17:21:27 GMT  
		Size: 14.7 MB (14672721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
