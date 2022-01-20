## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:70ced55dcff723418952067f9fe62373c25b581f8c207ce32b04df3bb3b19e66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:577307ba4b2eb382bf775435d42a07a6c59d9dbc31d50d5ad3fbb05805b01d2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329483266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95976ae34827ae62996b5a1661c022a8e62bf0eed21453373d8e1dbd3bcfdb25`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:29:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:30:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:30:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:30:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:30:25 GMT
ENV ROS2_DISTRO=rolling
# Fri, 07 Jan 2022 04:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:31:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:31:02 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975a65f4140cd95ee881ea97ea69c6a4281b69ecedb9e71cfc8facffcd4fced`  
		Last Modified: Fri, 07 Jan 2022 04:41:04 GMT  
		Size: 70.8 MB (70809014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aa7e9a462136248a1bab745e0ef3700e8455754a798add890def6b37a005b`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 250.8 KB (250795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d26a9439e09a0948d815314f26bf67505a8c65acc36c1488d8811573545c1f7`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1f316243ac1be85ac6dfa37b569d24ecef99f9ea08145931fc5a90b217258`  
		Last Modified: Fri, 07 Jan 2022 04:40:57 GMT  
		Size: 22.5 MB (22516472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda97e6ba89e5697ee900949aca16772f1798a21c3efb4ec433b8358ffa49841`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506852a7d2749b096216e1eadd03cbdfb60e96c86df52beb9295501d72641cc`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fb23629f42df10a8ed83a391805de422303358d7f7583266e40ea461996689`  
		Last Modified: Fri, 07 Jan 2022 04:41:33 GMT  
		Size: 78.6 MB (78594346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5166b5d0ce1da97b2ae850409848cd27da7262ea251f7e2567978bce841dcb`  
		Last Modified: Fri, 07 Jan 2022 04:41:23 GMT  
		Size: 17.7 MB (17702440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b649a44b9f39f22936fa3bf0e53e12a9aa409718e55b72cb1d0fd8c036ca0cb0`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c1664b818cf888cb72dcb072a35db1fdd9a6824460642b03d06d407d2f31321
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316632869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb103f51cb80913bf1e2ad173d23a2f3f546032366141a5df1dbd19a8fb510f1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:29:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:30:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:30:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:30:31 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:30:32 GMT
ENV ROS2_DISTRO=rolling
# Fri, 07 Jan 2022 03:31:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 01:55:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.18.0-1*     ros-rolling-demo-nodes-py=0.18.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 01:55:17 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30c74104597caa34b1cf8dbae71571ea6b16babbfd42dc0307090ca2fc8bcb6`  
		Last Modified: Fri, 07 Jan 2022 03:41:37 GMT  
		Size: 64.9 MB (64932455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba76342cba00f5b67fb766da3e232f9c1315ec60d929e502e588ffc1c13a0db`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 250.7 KB (250740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe848460e818385e527aacdaedad1d93510afdd9191a5ae514aa49666452a`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f842b26fd064cb8a18f71dd7718b127b2c05f1c484e87d46e363d70879d09`  
		Last Modified: Fri, 07 Jan 2022 03:41:31 GMT  
		Size: 21.8 MB (21833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6032ab55393eb2858b6d6a300bcfc7028fa5224f31798295a76cc740f40924db`  
		Last Modified: Fri, 07 Jan 2022 03:41:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb29997726224017b910e6c1b6ae50ee12d9e483506510d5529767b20f0ba16`  
		Last Modified: Fri, 07 Jan 2022 03:42:07 GMT  
		Size: 78.3 MB (78324741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac790522a79686a9a526ae5900dac7bec2fb522b582df444a5af4a14adec50`  
		Last Modified: Thu, 20 Jan 2022 01:57:21 GMT  
		Size: 16.9 MB (16907150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06a97f40c19eec1b082d57c66f04029c9caaad93b377f662f1eb266938f4ff`  
		Last Modified: Thu, 20 Jan 2022 01:57:18 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
