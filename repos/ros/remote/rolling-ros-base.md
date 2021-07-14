## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:58425c1b41f2292db91065236cf60785a1f6e30049292e966ba14b9590d9e48c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2a59ea0be0266569aad467e34390165f4dbc36f566e43091cc9f25e27922c685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232540777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd67dccbdfe5d95843c4ad1553f2b21d19d3b59ac1a56e359223af4d7edadae2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:27:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18c965f24291e45d1a63af72591fe112b32ca55c67d28e01d9028ed2ee633c`  
		Last Modified: Wed, 14 Jul 2021 02:39:44 GMT  
		Size: 70.8 MB (70796766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd11c5e8bf5476993b5e5db2880634369156fdc6d4dd54570b76ab74aa0de09a`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 238.6 KB (238614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4578383d135282389ec968781336ef5339ceeaeb77fedad4244339447a262e`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585de5ef0121eab1bca194101deba13a59c5dd66731a7988ef18cff8066ab4ca`  
		Last Modified: Wed, 14 Jul 2021 02:39:33 GMT  
		Size: 22.2 MB (22164073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

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
