## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:41ed09bfe510d8f1917a2c19fff4def4e5530b3b5584955a3ff4f97066b42f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:38f52106bd035bf0f6b11f3a4a7cb5df16ba7f907b8d4929c6e77ad855be9a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.9 MB (328878897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f8ebeb07a93dcd1df45cf05457b81dcc130e9b3a2f7be9c5fca06e9880ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:44:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:44:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:44:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:45:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:45:19 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:45:19 GMT
ENV ROS2_DISTRO=rolling
# Sat, 16 Oct 2021 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:41:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:41:34 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29283b46cfd735b60062e5f91075c6f2ea843931acc59c14f37eb39221dd2b8`  
		Last Modified: Sat, 16 Oct 2021 03:52:44 GMT  
		Size: 70.8 MB (70796841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e9ed06c574509d9c0bb9d4a2c44f6ff114c1077e353cba7362c84cc4e6928`  
		Last Modified: Sat, 16 Oct 2021 03:52:34 GMT  
		Size: 246.5 KB (246456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610fdb8a0efd75ac022b32e5bd0ab2e949a04010b31b2a1f1955479553203b4`  
		Last Modified: Sat, 16 Oct 2021 03:52:33 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5624b902d835e1730c98d69e69b0b0b7426d0fa45bb0bfc22612403589e0b`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 22.2 MB (22184954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33db4091cb9bc6536ddafd99784ef2739f5ab1f90d5ffa63bb125186ec7dfe6`  
		Last Modified: Sat, 16 Oct 2021 03:52:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b8ed699742f417db6e46477f6cbbbd143b369a666b9504d8fd3ef42c6b4827`  
		Last Modified: Sat, 16 Oct 2021 03:52:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac122dc08231f6b44fa9d50c299b4f9721a1351adba204bb58863fbf0fba1b14`  
		Last Modified: Sat, 16 Oct 2021 03:53:13 GMT  
		Size: 78.4 MB (78428391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd9582a655c0588ddd7b3cdbe066a85156e3cace0a3c7d2cdb8de6543b4a6b4`  
		Last Modified: Fri, 12 Nov 2021 01:42:41 GMT  
		Size: 17.7 MB (17701920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65cb722cddccca5b5b84c3c341e411432269ca99d7fb35dfb562c3c99f78e23`  
		Last Modified: Fri, 12 Nov 2021 01:42:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:69fd36b6bc76e9a69e1dbe9fd7baba4175c11591de07f6cc6dec6469aa41104e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316060914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a943606e0177bd34cc3f1cad5cbc775f7c190ab64f981346b25b13dda8f229f1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:38:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:38:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:39:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:39:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:39:13 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:39:14 GMT
ENV ROS2_DISTRO=rolling
# Sat, 16 Oct 2021 02:39:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:21:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:21:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d3c7da3194f2ecfb190e30268c8d48f6234b20e8aec520afaabc90cb86057`  
		Last Modified: Sat, 16 Oct 2021 02:52:27 GMT  
		Size: 64.9 MB (64922124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605cd44436c348c295974385f97270bbfe47c80a3004ac7e1470ecd75955075f`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 246.4 KB (246396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09852bd281240a5a11ad01942f7d7b2d78bc9910b588bc5b648036202ba2aa`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fed610107408e1af96e0fc9d2c3da4e93ff305321078387b8a569e0e297c8`  
		Last Modified: Sat, 16 Oct 2021 02:52:21 GMT  
		Size: 21.5 MB (21518723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b23a5fc866c0d86236bcc6617a57feeec98579b0653da4ec56e140a78395fc`  
		Last Modified: Sat, 16 Oct 2021 02:52:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cd393f58617c01a967f7b190061a1be8d33528cce968c447c4c5f437fa1378`  
		Last Modified: Sat, 16 Oct 2021 02:52:56 GMT  
		Size: 78.2 MB (78154328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d2314c5b843696dca1afa6c872380d59c40733a274735e8d0716614632bf53`  
		Last Modified: Fri, 12 Nov 2021 01:23:23 GMT  
		Size: 17.0 MB (16961150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34424424413d3f4a7b9136c2085242a96bcfc3cb8ccf15117fa3328694e674d5`  
		Last Modified: Fri, 12 Nov 2021 01:23:19 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
