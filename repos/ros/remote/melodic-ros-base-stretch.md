## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:0d187ccf28c3c6c5ac38b12054d115c9e6ded1de2c631f735955f05863eeed03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:dcd571a8292412c9f7282c50521dc6bfb444b7d34a33f37e308a877411eb2850
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.8 MB (447750887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1840fa34f6b5d809b6a6109148c2a36508a162e4eadb8df3073a1e6b01a0e13e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:36 GMT
ADD file:5f8ab4280b54d91475c84e497163ec05aabb5a9f9b9de687d38fda535ddc29b2 in / 
# Fri, 12 Mar 2021 02:22:36 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 14:04:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:04:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 14:04:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 14:04:53 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 14:04:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 14:04:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 12 Mar 2021 14:06:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:06:36 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 14:06:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 14:06:37 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 14:07:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:07:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 12 Mar 2021 14:07:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16cf3fa6cb1190b4dfd82a5319faa13e2eb6e69b7b4828d4d98ba1c0b216e446`  
		Last Modified: Fri, 12 Mar 2021 02:29:57 GMT  
		Size: 45.4 MB (45380216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3172cbec46580974c66064d5b95445203edf7f74a5ea53de5e494d4755a1eb25`  
		Last Modified: Fri, 12 Mar 2021 15:05:56 GMT  
		Size: 6.9 MB (6869236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbd42163a149ac542a7f9411b61635d5944e1082b809b3de759a61956387c58`  
		Last Modified: Fri, 12 Mar 2021 15:05:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a61e2edb7c90e5a9297a488f715836892d3381b3d396118a1ad7f800808eba`  
		Last Modified: Fri, 12 Mar 2021 15:05:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f8333c20c04c61e13156ab79655d4394ff3cdebd8fd2e1454d4fac847e1a03`  
		Last Modified: Fri, 12 Mar 2021 15:07:02 GMT  
		Size: 270.0 MB (270039735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7607f28b1b4513d274712f5a92e3776a809e2a220cb6ecbb6573742f1bb067b4`  
		Last Modified: Fri, 12 Mar 2021 15:05:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83368202c2ed781144da1f79a934f5223bdd3285ff85449a2a64769ff5dc6a0`  
		Last Modified: Fri, 12 Mar 2021 15:07:33 GMT  
		Size: 70.2 MB (70152551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf4ec269652984339c3a4ce8ed6b4ffc7156137f009f781f22419f93a556d2`  
		Last Modified: Fri, 12 Mar 2021 15:07:13 GMT  
		Size: 248.2 KB (248218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d4bc005a4d74726bc704732b5cbcf4b11082710df13e8ee248b40a6b9063a7`  
		Last Modified: Fri, 12 Mar 2021 15:07:32 GMT  
		Size: 55.1 MB (55059112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:15611f00b539a46e1b78413b49ba5573eb3f441bfd07c00e6ab094b1b52e33df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.1 MB (393060424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2915a9862c7da472bf777090cc112700269f8973bb715b5962fd9c4aeb2651c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:56:48 GMT
ADD file:3d59786321ef76584460518105748706e36cd0b833f1d542702f9e238073f63b in / 
# Fri, 12 Mar 2021 01:56:54 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 19:04:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:04:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 19:04:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 19:04:33 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 19:04:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 19:04:35 GMT
ENV ROS_DISTRO=melodic
# Fri, 12 Mar 2021 19:07:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:07:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 19:07:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 19:07:22 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 19:08:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:08:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 12 Mar 2021 19:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:690bb835f855da2bebb5afc2671951a9cafcaae8e3751eaa3ef8536058581b9d`  
		Last Modified: Fri, 12 Mar 2021 02:03:51 GMT  
		Size: 43.2 MB (43177463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c944cbfa5496d5ec8871cc49f314bceee143a6567e79de571e0ccded6bd884fc`  
		Last Modified: Fri, 12 Mar 2021 19:28:02 GMT  
		Size: 6.4 MB (6442965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66de9f5234112384d19c720628cd390e87e645acafe7ab660da6b42ac8f3073e`  
		Last Modified: Fri, 12 Mar 2021 19:28:01 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c877ab2baa655d397dc3dfe4956d5a942c97d1087b7ad617fbd51f06c150b79`  
		Last Modified: Fri, 12 Mar 2021 19:28:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4d24f6566c6ea7a51e92754f0a2ee81cf644f13bb71c219d87a4eb6a0410e`  
		Last Modified: Fri, 12 Mar 2021 19:29:00 GMT  
		Size: 225.1 MB (225102874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5422e7a4fe1f9f372f5e180ac66843063feb47b808b3915a2a2d89522e93121`  
		Last Modified: Fri, 12 Mar 2021 19:28:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc6cff16269c9470d4b2c12870ceda92c6fe744dfcb95c20b3bc40750b1f901`  
		Last Modified: Fri, 12 Mar 2021 19:29:28 GMT  
		Size: 64.8 MB (64841411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170046e2ac52c4f02ee222d4c8c2c36a594c009f818037bf00f4e6d8ddf19de`  
		Last Modified: Fri, 12 Mar 2021 19:29:12 GMT  
		Size: 248.2 KB (248222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3253168b20d470f5a0d79df6c9f8c654da54472d6ede65c8f4a0b66bf0bbbf22`  
		Last Modified: Fri, 12 Mar 2021 19:29:25 GMT  
		Size: 53.2 MB (53245669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
