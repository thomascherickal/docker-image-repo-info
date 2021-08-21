## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:990cc51d99701897f01c29dfc020f6a00c81ec0ae3f7ab7191c9e925a401fbb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:0419b55655a8a9788ef62f230ba0c5c0995210c7324d7219d9cb4e74f318bb77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.0 MB (326047946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68d462b62bcab867a18dd90da22c7a31a8a05a81712003a2346f4272d9f4fb7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:09:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:09:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:09:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:09:39 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:09:39 GMT
ENV ROS2_DISTRO=rolling
# Tue, 27 Jul 2021 01:10:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:10:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecfae6e660eea869e3a4f0b50e02e1f4d59061ecd4f0183ae66f147a79b142`  
		Last Modified: Tue, 27 Jul 2021 01:20:31 GMT  
		Size: 70.8 MB (70796958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9dc0d5adb890f7b8a3773d5280d5a49fc76acb26a178acc8625286d67ffb48`  
		Last Modified: Tue, 27 Jul 2021 01:20:21 GMT  
		Size: 239.9 KB (239910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72269352c197138327479f8993a3f63c4d1e1f551153f8892c4b0e0655b7cda`  
		Last Modified: Tue, 27 Jul 2021 01:20:20 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c9e6f758bbce1c98b1b54d6df1e86f651ececc09089ad70ff299c3251599b`  
		Last Modified: Tue, 27 Jul 2021 01:20:24 GMT  
		Size: 22.2 MB (22162528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b7e5b68d937de167626e1fbf8f8aa89e0b98f223f92214e751b6bc93ac02ae`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae277910ca8875daebb4c39ac8f951db856449b3de053bc5fd2b5823c5ee57b6`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f022dbe32fe832b14ad9e12583044b8108dcef7b9a90ffdbe21c579aa88700df`  
		Last Modified: Tue, 27 Jul 2021 01:21:00 GMT  
		Size: 78.4 MB (78413507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81921727929ab00ed80fb90e17e0e83df6fedf858d8a2addc82b2ae712ee73c1`  
		Last Modified: Tue, 27 Jul 2021 01:20:49 GMT  
		Size: 15.1 MB (15095090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1189306f1356224513996d689a685113a9dedeee1a681978f8fd363a6c0c44`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f1250cc8adbb1af04bfa1609832656cee28a8356680f564729f5eb2a6fb7a299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314248509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b02289d93836ace703f870dfbceb86842ef410a8cddbd8dbdfa258e700a13bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:14:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:15:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:15:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:15:04 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:15:04 GMT
ENV ROS2_DISTRO=rolling
# Mon, 26 Jul 2021 23:15:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 00:47:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 00:47:18 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466268875e4dd8ad642170e2c1132182e9c266799d18eefce6c20354351aa816`  
		Last Modified: Mon, 26 Jul 2021 23:27:46 GMT  
		Size: 65.1 MB (65137818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60d1728b6b23474a432d8ffaec35473daa09949408fac1589d8a7182f815ac`  
		Last Modified: Mon, 26 Jul 2021 23:27:36 GMT  
		Size: 239.9 KB (239911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbbc3fee7c944f77b2c41db5aca4329fc0bc2e4a994721160762d54ecedd`  
		Last Modified: Mon, 26 Jul 2021 23:27:35 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d260efcfbe512e4fb840d5ea90945601804ede2a216902a171de34573131b`  
		Last Modified: Mon, 26 Jul 2021 23:27:39 GMT  
		Size: 21.5 MB (21500860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2268c306b1f6a009ee0c79d6c1944981ed7dcd117e4e2097ae6bb68699573a`  
		Last Modified: Mon, 26 Jul 2021 23:28:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff82791f9fea2e59a2957e9d5aab45bf09b288a72892251ab9de125d71194c9c`  
		Last Modified: Mon, 26 Jul 2021 23:28:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a209440aeee45f4c1770fcbdde5de1d5c53a624af51ca0ab250d77e8d20c2767`  
		Last Modified: Mon, 26 Jul 2021 23:28:21 GMT  
		Size: 78.4 MB (78370885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fb53b43a27675601a6fd0fdf8bc19718d53ef84cc49756dec43c8b73c6d330`  
		Last Modified: Sat, 21 Aug 2021 00:49:39 GMT  
		Size: 14.7 MB (14704601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ec5035f5b4e3519133a2ea30b97d2599a7493c1dd926d6eaa32c5f564f755c`  
		Last Modified: Sat, 21 Aug 2021 00:49:36 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
