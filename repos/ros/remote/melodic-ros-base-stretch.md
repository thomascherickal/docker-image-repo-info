## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:d05635c7520e2ccbec122911ae69da341b5d457e1b9188a1b0ebbc7c6ab80e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:dae34e8594a8c322ac2dc7403a084bf5e4f4d729f0db41d65697c534767b3ae4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.9 MB (499917644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04da5b50c44b2e66788ca85088abc106e99db345e77a56b714f6ec0e8f68bcb7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:49:37 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:49:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 01 Feb 2020 18:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 01 Feb 2020 18:50:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:50:37 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 18:50:38 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Feb 2020 00:04:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Feb 2020 00:05:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Feb 2020 00:06:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 06 Feb 2020 00:06:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Feb 2020 00:06:14 GMT
CMD ["bash"]
# Thu, 06 Feb 2020 00:06:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905ca7a93e1f1f1e5a3c9d5dacdf39395a357b216f42962d54cb9f2f2779419`  
		Last Modified: Sat, 01 Feb 2020 18:59:03 GMT  
		Size: 10.5 MB (10476666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d9067426f73e53072c040a66d4e587fa9badca3da3aed990b6ef8afe8385b`  
		Last Modified: Sat, 01 Feb 2020 18:59:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47253481cad39c6f079e90a602a37b6638204f66869e48320e2d414b8ec82be5`  
		Last Modified: Sat, 01 Feb 2020 18:59:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822fec1fbb983df499d36a4c4325090bc1538e03ea008262104c269ccf6d6dc4`  
		Last Modified: Sat, 01 Feb 2020 18:59:18 GMT  
		Size: 64.8 MB (64771303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16863f4abfb019c6e8a8fea1c6e62b6143066c7f5e93a79efe3e9b651ebc248`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 416.3 KB (416299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16c2d9ace030f8cf7130554cca720123d8d98ac042030446e8e63d2fed7575`  
		Last Modified: Thu, 06 Feb 2020 00:24:16 GMT  
		Size: 270.4 MB (270396052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dc5fb275b853031a6119ad6970232236aa67ec1091eb754ef605ddcdb0ec0`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989e70d294fe3d20b5496caf95ff8bbbd3a87f2767957b524094176593b4b0`  
		Last Modified: Thu, 06 Feb 2020 00:25:02 GMT  
		Size: 108.5 MB (108474848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2faade4fe6adba2f9cca34336cbb2d155e8fe412c5153563cd9a55cea7147697
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.0 MB (443016659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9445d40e3b8f06c7cb6d2de0edbadeba82e5a7da4755733ec346c9dfa9d632`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:31:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:31:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Feb 2020 14:31:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Feb 2020 14:33:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:33:23 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:33:24 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Feb 2020 14:33:25 GMT
ENV ROS_DISTRO=melodic
# Wed, 26 Feb 2020 14:33:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Feb 2020 14:36:54 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:37:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Feb 2020 14:37:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Feb 2020 14:37:12 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec93ccfa7a93f6e8e92bfb6a4612d88201a991de0eeccbf0f0bf911e494b010`  
		Last Modified: Wed, 26 Feb 2020 14:46:38 GMT  
		Size: 9.8 MB (9774844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d47cc5c856874753256905adae1cafc7bbe555293057734a15adff043ad552`  
		Last Modified: Wed, 26 Feb 2020 14:46:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8904c2c29a9d325e34d20fc23a9bf0424e4011a33a408e44efc9d3a7afd762`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd405032f54a80c542f1c495a333e79235726b6bc13a929b1cd5b8c1857cf4da`  
		Last Modified: Wed, 26 Feb 2020 14:47:00 GMT  
		Size: 62.1 MB (62091345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22cef13f13ce297cd764e86e8e695631eb4f9bd35437f30cb2fb4121836e4f`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 426.5 KB (426457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c556607af67c09197a3819a5d4186a8a16161d13034880bcfa9896a95453d8ee`  
		Last Modified: Wed, 26 Feb 2020 14:47:46 GMT  
		Size: 224.6 MB (224601602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61457eaec54891acb526a2385adff233378c15c155753857cab7397dfce078c`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d522db6c8689265e2a824a336e54ef5e1d066934054d93dd8a56e3fb7098a9`  
		Last Modified: Wed, 26 Feb 2020 14:48:16 GMT  
		Size: 103.0 MB (102962444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
