## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:d2bd8d7ae1bc12bcc3c99e4e1dce22de2e4f23129cd989eb2be03ea113d33db6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:81a25ad83d26c179eb9b63b60933fc77f20c8cc68dfae1b168b542510709ffb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322553266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:343d6ece9ede76a8dbc169b285948d227c28b301b0ab37f47764f57ece3ec6b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:15:42 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Jun 2021 02:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:16:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:16:28 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:16:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:16:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:16:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:17:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 02:17:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:17:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Jun 2021 02:17:25 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Jun 2021 02:17:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:00 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada5f16a026eab8a221d51db2c20e9ea37c3072a0b2c281604fff5aad6696b1`  
		Last Modified: Fri, 18 Jun 2021 02:32:25 GMT  
		Size: 103.6 MB (103613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb5ea6029f88f11c4d97cb320027f91b4fbfdd58ae7180d2bf1bb5c23d00f35`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9f55b4fa18ae28d3d3490dbf2e89ec6b258acaced76fab09c769e7c21738f2`  
		Last Modified: Fri, 18 Jun 2021 02:32:48 GMT  
		Size: 66.6 MB (66550544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9274976ef70285b0e42376a86ed012534d5a01283c03c9fdda991545c3c11`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 234.4 KB (234425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10677ba132e2f8550410ea57e748edc342b44c8445b594c14a698f113c9ffe8a`  
		Last Modified: Fri, 18 Jun 2021 02:32:35 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d6631a8510e42592ff9485f745b27133e502c2ba2c621ec936e3ac56caab4`  
		Last Modified: Fri, 18 Jun 2021 02:32:41 GMT  
		Size: 22.1 MB (22095295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67b827799f8410ffac85eacd7ba4da0d2375ae6a99c5c45f8c2f7688f014371`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe4710e4bf4c1167669a16f859d5cdb27c0eecfe90e01110558b697210a403`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada466ddc6b96b7af9abc72a23c6e7cc55a74162f8fa73ce97996ac018ea43a4`  
		Last Modified: Fri, 18 Jun 2021 02:33:24 GMT  
		Size: 78.4 MB (78409357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6db6cddc1ed7a70ccdeb1610359ec4b968e5536cfe49642b1f063dd9d4d6f9`  
		Last Modified: Fri, 18 Jun 2021 02:33:07 GMT  
		Size: 16.4 MB (16362214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf26bba415264851b5c953e79eccd6bdf209638624ab654fc27475f021aeef7`  
		Last Modified: Fri, 18 Jun 2021 02:33:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21dbd174709b05d963c775428d818c6859e7e0333569017dde41c553d52c9d29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314947249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1d258435ff91e645e428026031524073e7298d90a9588a3f2cf5869dada9a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:41:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:41:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:41:28 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:41:28 GMT
ENV ROS2_DISTRO=galactic
# Wed, 14 Jul 2021 00:41:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:42:09 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb317f13463f02047277be9351ec1be0004beab4e6bb9fee342f11ea8f4914`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec27dc4a7abd2df6cdd4705ba4380601e0ba406454fd3a386422f8f07c97ca0`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e453588761a1c6c9d89a74b2f49c7b8bab3629b5665f6cea21489228dddec0f4`  
		Last Modified: Wed, 14 Jul 2021 00:57:49 GMT  
		Size: 78.4 MB (78368862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6447c99abc27d97a49b6e75f2dcd5cfac1bce156b1d593e436a87fef8365e3c9`  
		Last Modified: Wed, 14 Jul 2021 00:57:31 GMT  
		Size: 15.9 MB (15889992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc287c18aa593411cc80a90e25dcad46077e7c0a28af363b9eec15af1ce8dd3`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
