## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:b65363885bae56e89772a86a58cff65f7aa23848e01df6d07072cbd1c544c36f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:aada9dce3c97d5d317837a3a0f146b85b33ed41947e0d3d79bef080500c91d73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.8 MB (447781896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6bc0134b231fb47ded22b214c6de910e3a7ed2a1be29ddc112b12cb8d7dfdd9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:12:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:12:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 27 Mar 2021 09:12:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 27 Mar 2021 09:12:24 GMT
ENV LANG=C.UTF-8
# Sat, 27 Mar 2021 09:12:25 GMT
ENV LC_ALL=C.UTF-8
# Sat, 27 Mar 2021 09:12:25 GMT
ENV ROS_DISTRO=melodic
# Sat, 27 Mar 2021 09:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:14:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 27 Mar 2021 09:14:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 27 Mar 2021 09:14:09 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:14:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:14:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 27 Mar 2021 09:15:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d657504ffb8f628d70a2b1e2672e16b95f6eac895057e4cdcb97e09f862a1b09`  
		Last Modified: Sat, 27 Mar 2021 09:26:42 GMT  
		Size: 6.9 MB (6869187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa6cca370d6196ae385348a9369c89f41ffa9578e97dddffed55be61d6e0e62`  
		Last Modified: Sat, 27 Mar 2021 09:26:41 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404a516aba8bbb9ba24fdc7ef19705ce8dd84915cf4cd2986249f95c22db251`  
		Last Modified: Sat, 27 Mar 2021 09:26:41 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb5474c655269c720249df5c38af05416a1d5e3d33019bffbcd827297ddd6c6`  
		Last Modified: Sat, 27 Mar 2021 09:27:27 GMT  
		Size: 270.1 MB (270070182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab44e97519ff7d9f42f3b133c7e261108a040df6ade9b5001b98fe56d831b1c2`  
		Last Modified: Sat, 27 Mar 2021 09:26:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b4e3577ec11e0ec0f964d88d42f446bc25d44365aac4bed90203216f05cef4`  
		Last Modified: Sat, 27 Mar 2021 09:27:47 GMT  
		Size: 70.2 MB (70152067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac8e068e3ef5cdbe90cbc04af49da34966533a80f7beab3646960b0267594bd`  
		Last Modified: Sat, 27 Mar 2021 09:27:35 GMT  
		Size: 249.8 KB (249815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f41d908f054838060d72326ca70b40b4d00631e57e56aae261e2569b448f9c6`  
		Last Modified: Sat, 27 Mar 2021 09:27:44 GMT  
		Size: 55.1 MB (55059313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d29f17800a0f3282123164d104ea92ac845bf9a3d68a602c7e36e857b6434c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.1 MB (393074913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ee088da844c4e6680b553ddaa91692033b755b7195a3144230b2994e29bdde`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:38:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:38:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 31 Mar 2021 13:38:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 31 Mar 2021 13:38:12 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 13:38:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 31 Mar 2021 13:38:14 GMT
ENV ROS_DISTRO=melodic
# Wed, 31 Mar 2021 13:41:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:41:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 31 Mar 2021 13:41:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 31 Mar 2021 13:41:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:42:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:42:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 31 Mar 2021 13:43:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9bcb4567c53b5710817f63af7d0c14a3dad36b823f3cc9f142434d89dd7cea`  
		Last Modified: Wed, 31 Mar 2021 14:03:12 GMT  
		Size: 6.4 MB (6442935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84574c97c15ff3c495faceaf91ec7efac2d7735c4fe357cc256339c4fe93410a`  
		Last Modified: Wed, 31 Mar 2021 14:03:09 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefd0949cc578f2b84114a09843d05b951725916a271d79c9e803a14021734f8`  
		Last Modified: Wed, 31 Mar 2021 14:03:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fafb8ecac1b3a711771dfd44718d41e04b5dcf0e3545af1cc8fc71a84905bb3`  
		Last Modified: Wed, 31 Mar 2021 14:05:04 GMT  
		Size: 225.1 MB (225114741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e8c7efe0eb7db52b3a500557e94b2126eb204eaf0deb2cb3356cdd72b378f2`  
		Last Modified: Wed, 31 Mar 2021 14:03:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae8b9ae40586f1c7f4a31c6f954c7fc823f68d3a1ca653021947d6561a88274`  
		Last Modified: Wed, 31 Mar 2021 14:05:39 GMT  
		Size: 64.8 MB (64841811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302c8cf265a1c9f49435bdb51988d9f6c72875806726beb107b029b0229c5b3`  
		Last Modified: Wed, 31 Mar 2021 14:05:15 GMT  
		Size: 250.5 KB (250541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bbb4913683784dfcd753468a71f92c352037f11cc8f978e91e1731b4591aba`  
		Last Modified: Wed, 31 Mar 2021 14:05:41 GMT  
		Size: 53.2 MB (53245478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
