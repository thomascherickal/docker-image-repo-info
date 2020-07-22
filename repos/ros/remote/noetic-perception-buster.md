## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:d7a3fbaafac3ac3edc7dc80da274a83ffc81a12ef1695c51d1a0f96a9f495fea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:04faa0314a17fc188c6a848620e2d4d5050b36437c8a05024ae2aedccfcc8db4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **967.4 MB (967447693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79eb6ede277295cc0655ea4db3cd30f64adbed9f14d6e8819c88dedb0702acd9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:16 GMT
ADD file:89dfd7d3ed77fd5e05f20a0ab631142207ae462f5bbd877f8745d3930c751d87 in / 
# Wed, 22 Jul 2020 02:03:16 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:36:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:37:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 22 Jul 2020 20:37:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 22 Jul 2020 20:37:01 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 20:37:02 GMT
ENV LC_ALL=C.UTF-8
# Wed, 22 Jul 2020 20:37:02 GMT
ENV ROS_DISTRO=noetic
# Wed, 22 Jul 2020 20:38:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:38:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 22 Jul 2020 20:38:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 22 Jul 2020 20:38:42 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:39:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:39:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 22 Jul 2020 20:39:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:43:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31dd5ebca5efc5e96a425402fa85e492b02c8fe757dfd3edfdea2a7c67322909`  
		Last Modified: Wed, 22 Jul 2020 02:09:37 GMT  
		Size: 50.4 MB (50390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2b4c3e83730582d8aa0afee630f3929243c3f8f169e5caec1fe3ede3cf6ac6`  
		Last Modified: Wed, 22 Jul 2020 20:49:13 GMT  
		Size: 10.9 MB (10889394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6406abb87b09a866ace4e9e958e5615813523268f2aec3d9dbfae13e5846cdc`  
		Last Modified: Wed, 22 Jul 2020 20:49:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b28b9ccd622fdbbf58e61bdad8f8c8dad46da7b9c7f8e34943e50fd8620536`  
		Last Modified: Wed, 22 Jul 2020 20:49:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf679ac616afd10160caa0e2749b11f0089dee06f00347db9e127a0acc7d9125`  
		Last Modified: Wed, 22 Jul 2020 20:50:03 GMT  
		Size: 238.8 MB (238811052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42f3a065603ac47dcbbd4973c26383f24086b994ff77ec0a96af63653e6ff74`  
		Last Modified: Wed, 22 Jul 2020 20:49:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da20226b027ad37f8885bcdd2e4c82a17f05df1ef0c7fd846d6fc7a248e0819d`  
		Last Modified: Wed, 22 Jul 2020 20:50:39 GMT  
		Size: 86.6 MB (86562111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c890a4646b0da35aff42dd24cc5b7aa05e2a8fab5829a33fbd7b3a6b78f102f`  
		Last Modified: Wed, 22 Jul 2020 20:50:09 GMT  
		Size: 207.6 KB (207642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcee7fdde209dea082685e77b5f848d6d3dffe257b466ddbd597bbe2922fb073`  
		Last Modified: Wed, 22 Jul 2020 20:50:35 GMT  
		Size: 76.0 MB (75966569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c467c1b59ab27d68e58e64be50ae187c866ccd51e7d9eae7eacb03924131c852`  
		Last Modified: Wed, 22 Jul 2020 20:53:26 GMT  
		Size: 504.6 MB (504618764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:663518598adae652ddced498b2d6ffdbea1df63d09822f855814e11e85c16c7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.3 MB (884295784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae05be021008ab157bb210916797addbd0ffbf68b033783c9061e213f3547826`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:40:37 GMT
ADD file:14b8dca0bc0e6dae2f0bdb018a3a4e6d8d041abd03d118ae27cf7a72668f4970 in / 
# Wed, 22 Jul 2020 00:40:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:42:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:42:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 22 Jul 2020 19:42:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 22 Jul 2020 19:42:43 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 19:42:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 22 Jul 2020 19:42:48 GMT
ENV ROS_DISTRO=noetic
# Wed, 22 Jul 2020 19:45:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:45:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 22 Jul 2020 19:45:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 22 Jul 2020 19:45:44 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:46:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:47:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 22 Jul 2020 19:48:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:56:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2b2cb832ad58353bcc4edbdd16023beb64ec7856b469d202975f8de836c6906`  
		Last Modified: Wed, 22 Jul 2020 00:47:20 GMT  
		Size: 49.2 MB (49168473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bfddc46c6ab775f75cbf1461903806fc5db4e18d330cdd1abfc805ff6bc2b5`  
		Last Modified: Wed, 22 Jul 2020 20:02:33 GMT  
		Size: 10.9 MB (10882062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd86b51a67e431b63da24473a298fdd0e8118500fdaa4f8c45b29277f45bb98`  
		Last Modified: Wed, 22 Jul 2020 20:02:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d91c81a64439007adea00a3e759d308ab2608db853ca6e5fd899dbbe327cf76`  
		Last Modified: Wed, 22 Jul 2020 20:02:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b4cd67fcc5120240a85d8be2e65ba4fe74da31a0ea31765137767c6ee51452`  
		Last Modified: Wed, 22 Jul 2020 20:03:31 GMT  
		Size: 184.0 MB (184047716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a78749a2f4425a34eb7aae6fe753da8e2540012c49dc5437b92c04d8471bb`  
		Last Modified: Wed, 22 Jul 2020 20:02:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b909393a587016cbf2e79a9882afcb640515c535c24e4a8490be6b907f616193`  
		Last Modified: Wed, 22 Jul 2020 20:04:00 GMT  
		Size: 84.4 MB (84355106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1601dbdbca7f3db0442a1d438c6b80fdd09ec4d1e51945982c75ebcbdc9e314`  
		Last Modified: Wed, 22 Jul 2020 20:03:41 GMT  
		Size: 207.7 KB (207661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c39b246944677e08ff29d154a4cdffdb18cbfade47fe049fefa4958021d8cb`  
		Last Modified: Wed, 22 Jul 2020 20:03:58 GMT  
		Size: 74.1 MB (74090182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163a7a55b934ffe5dfe5fe42d9da24fb0caaba864be2df06a23c22f2802a9fc9`  
		Last Modified: Wed, 22 Jul 2020 20:06:36 GMT  
		Size: 481.5 MB (481542746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
