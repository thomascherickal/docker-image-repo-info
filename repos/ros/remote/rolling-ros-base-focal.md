## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:f88661d6b3268ef40c6b75d4d6d2d6dc69d993b53e2c4e7e6498cd96ddf82aaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:38ddc87677cc7bafa7e79d4537365db18e9a870ebe35e51cd27274934c4723f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227799414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f840f83bd31e9a5d7d9b295c6b3fda49a0c27d1ec885e94ca6e4035b6c7aa286`
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
# Fri, 18 Jun 2021 02:18:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Jun 2021 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:18:49 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:19:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:19:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:de20d81bd4173a8339fec869e6e366ade6bc0fe364230a03c10df78cf96f9076`  
		Last Modified: Fri, 18 Jun 2021 02:33:59 GMT  
		Size: 103.6 MB (103615082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cb0aea3e4fffb341a10ccca49e0def7d1efbe7edbeacb6a0d83460d208b5a`  
		Last Modified: Fri, 18 Jun 2021 02:33:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837448df0815a613ee720a81c9f44ab668e5e4b2b2616b6f31a4495fea465839`  
		Last Modified: Fri, 18 Jun 2021 02:34:23 GMT  
		Size: 66.6 MB (66550472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420cde9136fdf7d018e6571536582bd69834d41d6f368fb1c18b4c250c02bcf`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 233.9 KB (233906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4da8004060a34a319a474c460b80e1554f49287d7b0f6caed1ad1fe56fc325`  
		Last Modified: Fri, 18 Jun 2021 02:34:11 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7a80f8badad65537ffae8798f29e730fa7544eec2776c97651295d0f70f5c`  
		Last Modified: Fri, 18 Jun 2021 02:34:16 GMT  
		Size: 22.1 MB (22112431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7643d34396ecaeaa9bf95bb0ba0d2b86c90b5909d9db960a1495d903e2709090
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221190595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c67d571630c4ed995384a018dc5a1c905b439fefd28ed0b010420b52d6e63d3`
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
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:43:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:43:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bfc647e1fd1ab9a4847f84273249517aaf1a4a26e8d4f53875340bffe0261`  
		Last Modified: Wed, 14 Jul 2021 00:58:51 GMT  
		Size: 65.1 MB (65137606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a24ecc4e22c8d052eab52f50488f5f3332fa2d2aac910ac6eaeb03ad3ff169`  
		Last Modified: Wed, 14 Jul 2021 00:58:40 GMT  
		Size: 238.6 KB (238602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d4894c659864a52419078687aa61e414bf7cf3621963bf4fa0b9f72c0665bc`  
		Last Modified: Wed, 14 Jul 2021 00:58:39 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518623f7b6c1c97adb1004f148e808e506f9dd89c4d4e14a08e22f66e18aaf1`  
		Last Modified: Wed, 14 Jul 2021 00:58:44 GMT  
		Size: 21.5 MB (21501974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
