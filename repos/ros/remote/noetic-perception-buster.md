## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:87f3c4e88c5e10b2cf2057da2883b088597738858081aedc2e7c946c551a77f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:2866d5a9fd9a5f6100f24c6445ca31d7c67a791a1d1de78e49ea311c624f9881
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.0 MB (968027873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92b05b8c11d0c1b4491b4717215140ddc602822b27a45f1c08fbad43c9a6731`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:14:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:05:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Jun 2021 19:05:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:05:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Jun 2021 19:06:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:06:38 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:06:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:06:38 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:07:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:07:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:07:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a04ce26341db0d6591d2793ca267552485c51f4cbb273019ac821d671266ce`  
		Last Modified: Wed, 12 May 2021 17:24:25 GMT  
		Size: 10.9 MB (10891745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f874a1d96f3564e1336fb9600729be2ea22b555e7af860074cfac35ef5aca5a4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c733261a68b07a3b86e48d99685861b97f39fa9c98eb8faa30f5794651d1736d`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271be76f2de712a4f3df979ae1d086ffd0f695f5786c1914807e6f68c00bf367`  
		Last Modified: Wed, 02 Jun 2021 19:42:16 GMT  
		Size: 239.1 MB (239077729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa12225bfbe392ebc8cd18c1353c6ff079a250c0c1077d87f1466cfbd29234d4`  
		Last Modified: Wed, 02 Jun 2021 19:41:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6be44022cfad412873932550fcb4c91fe1a2a38a00a3a6ce5dc2f26cb787ef2`  
		Last Modified: Wed, 02 Jun 2021 19:42:38 GMT  
		Size: 86.6 MB (86566951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f606a538348e9f7f068265e12126380e56c095c967e463d0f1eaf77176823b9d`  
		Last Modified: Wed, 02 Jun 2021 19:42:24 GMT  
		Size: 299.6 KB (299563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b093daee989ce1c0f63e8151bbb0c5cd4b6876a277b3be6867b2e766d1e7985`  
		Last Modified: Wed, 02 Jun 2021 19:42:37 GMT  
		Size: 76.0 MB (75975246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435c89077a0df30ca6ec5a5b09388704cb368ee693473db9b2c967a969c77435`  
		Last Modified: Wed, 02 Jun 2021 19:44:33 GMT  
		Size: 504.8 MB (504780986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:39730a3e078c75f54290461fb21399b6928b5cf3f1da00ba2e3329e4f913eef6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.8 MB (884774909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d82fbfe57b42fe230da293a099669a2d14384acb318cdc1bae83f80456c538e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:50:48 GMT
ADD file:ff9983cd659b3fc32ddfbbdeda76a971afd7d399e6d8b98faea3a9ead0e598f6 in / 
# Wed, 12 May 2021 00:50:52 GMT
CMD ["bash"]
# Thu, 27 May 2021 15:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:29:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Jun 2021 19:29:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:29:23 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:29:24 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:29:24 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Jun 2021 19:30:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:30:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:30:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:30:24 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:30:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:30:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:31:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:34:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c54d9402d498e45ed396b5b6fe836f55e4ccadbad745decda3e9f83d880bc677`  
		Last Modified: Wed, 12 May 2021 01:01:40 GMT  
		Size: 49.2 MB (49225351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef41d27594cb3f96faef94886e77e8683347542ba8089a62b566c5cf3844f61`  
		Last Modified: Thu, 27 May 2021 15:46:15 GMT  
		Size: 10.9 MB (10883255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e73149d5bb32c9d35c3e0e371d8188fd6cee9896d305d55d43a24bbcfefaefc`  
		Last Modified: Wed, 02 Jun 2021 19:58:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c50caeb0688dd6be0aa82ebb0fb6556a48fa1f792441b41fac4336582c8afcc`  
		Last Modified: Wed, 02 Jun 2021 19:58:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9e4db5443f46f1f3823ce6737931c7a65c041524ac2a56720926a5bcf57adb`  
		Last Modified: Wed, 02 Jun 2021 19:59:10 GMT  
		Size: 184.3 MB (184259045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fb0fb1cfa6f5541ddec8a8416f5e6f3d409eac4da0c9a1d445a06a1bda9079`  
		Last Modified: Wed, 02 Jun 2021 19:58:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8a10118734263d838c89d9a6eb15e62e2a30f8a2a928a29bdb68073ab3e191`  
		Last Modified: Wed, 02 Jun 2021 19:59:32 GMT  
		Size: 84.4 MB (84357807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6630ee78a55247d3a7e4775e2b65766ca9e9dd2d639bcc2cd112d04924120a`  
		Last Modified: Wed, 02 Jun 2021 19:59:19 GMT  
		Size: 299.6 KB (299561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898f051f82a93d2608e22811012a61ec8484e2a9833e81b991707f5a46be3182`  
		Last Modified: Wed, 02 Jun 2021 19:59:31 GMT  
		Size: 74.1 MB (74088052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4377940cbc10e5c05d8c5eea53d6daa0477266794684a2bba92cf595b7efc`  
		Last Modified: Wed, 02 Jun 2021 20:01:21 GMT  
		Size: 481.7 MB (481659427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
