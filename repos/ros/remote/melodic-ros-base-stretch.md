## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:bc8d89b50cf99d74248454f44e77f64abc8f9e8e881b9ce0ddabc7370d210419
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:53e4163895e0b157de0df064dfd4d41f8b737759d2e6a82479552390e9ab1023
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.7 MB (447694466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a269134e73345a6af1ff9634484f665c1d9501ab13d6f7488abdd8976d8a717`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:33:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:33:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 11 Dec 2020 19:33:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 11 Dec 2020 19:33:09 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 19:33:09 GMT
ENV LC_ALL=C.UTF-8
# Fri, 11 Dec 2020 19:33:09 GMT
ENV ROS_DISTRO=melodic
# Fri, 11 Dec 2020 19:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:34:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 11 Dec 2020 19:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 11 Dec 2020 19:34:32 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:35:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:35:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 11 Dec 2020 19:35:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de16d0f50b4374ec5823bc92988f1c2a778f1488b91506a4c32e9d1113484162`  
		Last Modified: Fri, 11 Dec 2020 19:45:48 GMT  
		Size: 6.9 MB (6867507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e746a7af5ec95aad4a3f31c82da9419cfdb13fcaed8e4208603158759f5cf11c`  
		Last Modified: Fri, 11 Dec 2020 19:45:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625f4ae7c99ce503a8e21550bd9b5a979988fb68d7c66fbadb69176e4418cdcf`  
		Last Modified: Fri, 11 Dec 2020 19:45:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3744e199296c0c17c5a8e3df35bd85f751da56707156b925b7b000d5737d718f`  
		Last Modified: Fri, 11 Dec 2020 19:46:40 GMT  
		Size: 270.0 MB (270002618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8741ee1a7786ebcda2770d3ca58252c17705e05df5150d3404d619f284782efa`  
		Last Modified: Fri, 11 Dec 2020 19:45:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c24d2b0be032d503a8617c57a56db106c7e9539df0f90ca1ced755924cacb74`  
		Last Modified: Fri, 11 Dec 2020 19:47:00 GMT  
		Size: 70.2 MB (70152806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d84fd2be2e2c475ae0e42692a2ec4b009fa446c7427b59dbeeefe7bc03a7eb`  
		Last Modified: Fri, 11 Dec 2020 19:46:46 GMT  
		Size: 238.5 KB (238493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27843f82639160d7c2f56a4da4f79a000dbea007be4c2fd4301fcef7283c1d91`  
		Last Modified: Fri, 11 Dec 2020 19:46:58 GMT  
		Size: 55.1 MB (55053618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1669f95cc61a447b60b781ac504716880b8dee7c4355c1d26972836dd28ac23c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.1 MB (393059317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856e59688b267c9f5056b614778925725d7a89fa406214815c13761e06e25f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 09:12:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:13:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 18 Nov 2020 09:13:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 18 Nov 2020 09:13:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 09:13:08 GMT
ENV LC_ALL=C.UTF-8
# Wed, 18 Nov 2020 09:13:09 GMT
ENV ROS_DISTRO=melodic
# Wed, 18 Nov 2020 09:17:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:18:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 18 Nov 2020 09:18:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 18 Nov 2020 09:18:04 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 09:18:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:19:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 18 Nov 2020 09:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92602d4f5b35fbaf1e8fb6e411e04e5971ce33abe3c7fd5964643892b701db93`  
		Last Modified: Wed, 18 Nov 2020 09:48:11 GMT  
		Size: 6.4 MB (6440978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf801218bf713e927fb087f64d89fe28628b81fd8acd57df9e4ba24ba6c30ef3`  
		Last Modified: Wed, 18 Nov 2020 09:48:10 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48643aeb8ff25cf211053dc193b030b253350d3971e2e58d453851c9d6e2e7`  
		Last Modified: Wed, 18 Nov 2020 09:48:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264bb6a4cb2e6ef5b80b5c02c9dd2dc4f790e1ad5c5e9db55d0014d33248f173`  
		Last Modified: Wed, 18 Nov 2020 09:49:09 GMT  
		Size: 225.1 MB (225086213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7356b45f618401b91d614bfe17badbbe1fedbd8b057ac7d88df4f9045be4`  
		Last Modified: Wed, 18 Nov 2020 09:48:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c5c31a03ea726417639eac21a23e2910ccbe53394b0219a7363783f6368f0`  
		Last Modified: Wed, 18 Nov 2020 09:49:34 GMT  
		Size: 64.8 MB (64842008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d19d2b200772b31d78fc0ff297f10c12f7f3d7ca10826491e95db88a1a20e`  
		Last Modified: Wed, 18 Nov 2020 09:49:17 GMT  
		Size: 268.6 KB (268580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56db4512c1a14af1ff014c4817e095576dd8fd9b1a58032793555b198bd3e2f0`  
		Last Modified: Wed, 18 Nov 2020 09:49:29 GMT  
		Size: 53.2 MB (53243709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
