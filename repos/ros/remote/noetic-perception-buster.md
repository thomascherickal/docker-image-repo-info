## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:1621d9355298f1b92319d8235b519b20cc59b304c830dc3d53911cbfe3119342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:809692431a8ca068012821f64abbd88d28919a28aebd1c9cc695eb8ddc378bb4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **967.3 MB (967261594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d45455ac94fd4a419759fd00066de8bfd09887af5587d286194fa9b91fb599`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 20:30:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:30:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Jun 2020 20:30:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Jun 2020 20:30:32 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 20:30:32 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Jun 2020 20:30:32 GMT
ENV ROS_DISTRO=noetic
# Tue, 09 Jun 2020 20:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:31:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Jun 2020 20:31:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Jun 2020 20:31:53 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 20:32:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:32:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Jun 2020 20:33:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:36:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2bc4e7737d5a2d3f5e9c833d870438ac7e50548abf7def874bc8ea95386dd0`  
		Last Modified: Tue, 09 Jun 2020 20:41:26 GMT  
		Size: 10.9 MB (10889380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4ff2824e647ea24bbff6408793f4f55d062652f3335695a415c55bd25912be`  
		Last Modified: Tue, 09 Jun 2020 20:41:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f982c829c7a71db4d03162f1624b3cbe81db4a2b15a6564fb9ec7c3aee69111`  
		Last Modified: Tue, 09 Jun 2020 20:41:25 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e21da98db453fa2714971f1395653edd6f2f4444e816ff2e1f1eb64fb8ced0b`  
		Last Modified: Tue, 09 Jun 2020 20:42:25 GMT  
		Size: 238.8 MB (238811177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1492e22c666d6f79fb430015c6a1ecd5cf0e03a036b3a2c1c95f1a66eaf7b80`  
		Last Modified: Tue, 09 Jun 2020 20:41:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910c19ba0ac7edcdff9c367e31c8832fa2773ccb40bab4b4a48e5385fd10def1`  
		Last Modified: Tue, 09 Jun 2020 20:42:52 GMT  
		Size: 86.6 MB (86563054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd25eb6ecc8af9898c262cb6fb7cc612dda5aaad982c5c1a4fdd493be975b75d`  
		Last Modified: Tue, 09 Jun 2020 20:42:29 GMT  
		Size: 194.1 KB (194107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14987723430ac78287b8cfd1e846a06fbe77ce5846b4bb0ae0cacd84fe41ee13`  
		Last Modified: Tue, 09 Jun 2020 20:42:50 GMT  
		Size: 76.0 MB (75966441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cd32eeb7b5f9e7570c7c17b9bb31aa7753ef7ebde7f9a9728bc3b76ce32f0e`  
		Last Modified: Tue, 09 Jun 2020 20:44:59 GMT  
		Size: 504.4 MB (504446096 bytes)  
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
