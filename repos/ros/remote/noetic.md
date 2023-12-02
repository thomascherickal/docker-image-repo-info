## `ros:noetic`

```console
$ docker pull ros@sha256:aa6a959e83c6ff2638b0f0250ee98e3fba3c99929c0a540f062391a4f87396be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:aa2cf66a0f6d613a56907d64c1325f9219b8b151d9d675bcfd85b6944e999572
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343162706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a5187b601f631f06e901329e1c6c9ee32ed4e1e4e235f6cd34d5af345f2cdc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 02:08:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:04:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:04:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Dec 2023 05:04:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Dec 2023 05:04:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Dec 2023 05:04:44 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Dec 2023 05:04:44 GMT
ENV ROS_DISTRO=noetic
# Sat, 02 Dec 2023 05:08:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:08:11 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 02 Dec 2023 05:08:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Dec 2023 05:08:11 GMT
CMD ["bash"]
# Sat, 02 Dec 2023 05:09:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:09:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Dec 2023 05:12:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc1327734170da8c4ae4171fb4248189d0691d6b4a3f01b09239c3e34688651`  
		Last Modified: Sat, 02 Dec 2023 02:20:57 GMT  
		Size: 1.2 MB (1198788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77125e61032dbbcd43c015fe756de97b5661bdbbf4f5219588148f651ae900c1`  
		Last Modified: Sat, 02 Dec 2023 05:59:34 GMT  
		Size: 5.6 MB (5553989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a419a7e57fda2f71bea1f99c76305ff5c0f72c3daed9b7440ca105cc25f1de9`  
		Last Modified: Sat, 02 Dec 2023 05:59:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a539454a4493a46768eee29a1cca9b7bfe5f4ab383e3669dde75e208d63790`  
		Last Modified: Sat, 02 Dec 2023 05:59:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83efb03e5f38cd29b39c48abc1bff37c30a6eec8221b87f6142d287789f8b90e`  
		Last Modified: Sat, 02 Dec 2023 06:00:00 GMT  
		Size: 177.0 MB (176955899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272aac7dcd28168b51bf129cec650d8e7e10fcecca57eb3b33f1111504ca93e`  
		Last Modified: Sat, 02 Dec 2023 05:59:33 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80787bbb4e152705c432d0f6be72de515673d0bd1e13c308b0b2b79dab42b28c`  
		Last Modified: Sat, 02 Dec 2023 06:00:19 GMT  
		Size: 50.9 MB (50940359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f0aa48fdc5b62a25880ad49af8531594ffd5a9eec93f28c14935098f88138`  
		Last Modified: Sat, 02 Dec 2023 06:00:12 GMT  
		Size: 310.9 KB (310898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0836b9b651f92dfca6a4c94574298a84d6bacf8a6bca656aed2e8303d90f6687`  
		Last Modified: Sat, 02 Dec 2023 06:00:23 GMT  
		Size: 79.6 MB (79616330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:17c021f745282198d89551e984956f5d32bf3b296d79d27c72eb5129feecba56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289222658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b381b176ed648076efff35763069250dfe58cad8d71f4ac9f298cae85523902`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:25:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:25:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:25:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 13 Oct 2023 01:25:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 13 Oct 2023 01:25:43 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 01:25:44 GMT
ENV LC_ALL=C.UTF-8
# Fri, 13 Oct 2023 01:25:44 GMT
ENV ROS_DISTRO=noetic
# Fri, 13 Oct 2023 01:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:28:12 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 13 Oct 2023 01:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 13 Oct 2023 01:28:13 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:28:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:28:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 13 Oct 2023 01:30:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a3643fb9ea7b4891593c2a71e53f70146f828b8896758ecc6804e843b3eb9d`  
		Last Modified: Fri, 13 Oct 2023 01:38:43 GMT  
		Size: 1.2 MB (1200040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d390fd421e090bebfad483fae5954c8ce4b3d98d6f7964b7d2af20febd3a8dd`  
		Last Modified: Fri, 13 Oct 2023 01:38:41 GMT  
		Size: 4.7 MB (4680598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f635e6735a4e72b10c5401661b398132793e75102ebdae3c1a4bb09369a9277b`  
		Last Modified: Fri, 13 Oct 2023 01:38:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc440f8be875763f266a01bddecd7e5256b0f7024383d18f3ac27b3eefca620c`  
		Last Modified: Fri, 13 Oct 2023 01:38:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8576e38b77aab0fa900f38b3857ac3f1f5f2f357b049bb4765eead409392f8ab`  
		Last Modified: Fri, 13 Oct 2023 01:39:16 GMT  
		Size: 157.4 MB (157433981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9929dceae2a7ac00be4bdeef95d2220d21923972182d5a0805ae6a130e9a5c`  
		Last Modified: Fri, 13 Oct 2023 01:38:40 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbc9c70d09913eddb72c3c4f69d3eacc75f42772407b3a7f1b83b8ab76e8609`  
		Last Modified: Fri, 13 Oct 2023 01:39:37 GMT  
		Size: 40.5 MB (40504496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4c4f8456ac317553d22cb6aeb19337c7ba56c832bd9ce3050a5666e4e67276`  
		Last Modified: Fri, 13 Oct 2023 01:39:26 GMT  
		Size: 308.4 KB (308391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11110f8ff52141ed436fcf91a65720ab159af26f35baf35ebec69235529767`  
		Last Modified: Fri, 13 Oct 2023 01:39:41 GMT  
		Size: 60.5 MB (60500564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e56292f13e93a79eaebd54ca1fc7cbce221cb489870c645c52c21a60984ae07c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322833438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ef0ff8399f8b8ffa366228b6c3a797d77f86744a8732f35f0389fdac3e32e0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 04:24:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:24:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:24:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 13 Oct 2023 04:24:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 13 Oct 2023 04:24:38 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 04:24:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 13 Oct 2023 04:24:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 13 Oct 2023 04:27:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:27:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 13 Oct 2023 04:27:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 13 Oct 2023 04:27:42 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 04:28:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 13 Oct 2023 04:29:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87696a1bdfb2280c9c8f032b8dad476643e285ea6a4daaaaf8dea807599345f3`  
		Last Modified: Fri, 13 Oct 2023 04:58:00 GMT  
		Size: 1.2 MB (1199301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c122b6409bbe49fd6863f4fe1b6c386aa8c0839b4d569cc6a7c864c54e4ebc`  
		Last Modified: Fri, 13 Oct 2023 04:57:58 GMT  
		Size: 5.5 MB (5532659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a917760d45f055be63dd5265386c3e099071676cbade870f5fad9204d410ad08`  
		Last Modified: Fri, 13 Oct 2023 04:57:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180f178865c356dfadb4351dd90e17e88bc0c96c7a5b00c3fa27f7a7a50854a6`  
		Last Modified: Fri, 13 Oct 2023 04:57:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70efcc630f7ac8f41932a95504f9faf4f5d3a98261ec78847c0b7895c7e38c55`  
		Last Modified: Fri, 13 Oct 2023 04:58:33 GMT  
		Size: 171.4 MB (171412015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7380be57882dd81c0bc849142d511e957f6f209e899d784c2169dd1268af381`  
		Last Modified: Fri, 13 Oct 2023 04:57:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03ae63d5fe1e840f0cc374100c4a33137e2c3862f567675d2a4f2a632ca68fd`  
		Last Modified: Fri, 13 Oct 2023 04:58:54 GMT  
		Size: 45.2 MB (45206478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78bb804d06a6c2affa7a4df0cb90051039812dd200a146925a447da4c03248f`  
		Last Modified: Fri, 13 Oct 2023 04:58:44 GMT  
		Size: 308.4 KB (308395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee77018c303d0f8b15482607876c85bd6f9bd91d7320f861f1146fc7f1e5f98`  
		Last Modified: Fri, 13 Oct 2023 04:58:52 GMT  
		Size: 72.0 MB (71972672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
