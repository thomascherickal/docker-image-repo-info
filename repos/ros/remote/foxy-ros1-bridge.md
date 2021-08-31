## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:cab0bb769bd317f011dc12d3facdca69f1fba414b2a7f3ae200641097bc09529
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:8f88647e50c42f9547aed07e6221d36c940d3eafa5ab5af8c2a9d145988e8f40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345516519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:894b70088b436277c4539f27a1d07ec70a49f0a5117ad7e582e04f26c65bca40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Aug 2021 04:52:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:52:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:52:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:52:14 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:52:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:52:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:52:56 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:53:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:53:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:53:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:53:26 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:53:26 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Aug 2021 04:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:54:08 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df88af5f8567a6f2cbdc3288e39989bafc21e16e19c1d0b21ec421155ba9d237`  
		Last Modified: Tue, 31 Aug 2021 05:05:42 GMT  
		Size: 120.0 MB (119973947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5d11ffe6ed85c308c8f7f83eb6779e2f81b2ce6c1328f73073878bc370843a`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee662a194237d1061dfbe6700abce9590c93e1d7c9fdc2c8030642fe89c07a`  
		Last Modified: Tue, 31 Aug 2021 05:06:03 GMT  
		Size: 70.8 MB (70844284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bba301f8377dd61e4e0a5652dea9356c35c590a01f73b857f8f9ee364e8a7`  
		Last Modified: Tue, 31 Aug 2021 05:05:53 GMT  
		Size: 240.5 KB (240536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e54ad7e3a8e61b43a65537755c95964771958deaa3af31dfd1a3b366ceeb99`  
		Last Modified: Tue, 31 Aug 2021 05:05:53 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f52ad208f27349b733c344754e7d5177833503ac3b8823c6416f1dba05b5707`  
		Last Modified: Tue, 31 Aug 2021 05:05:55 GMT  
		Size: 10.3 MB (10283858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768b198d04340eb2ebf05156bc4b5f86c6a05d3360700100c75a80dd9976da47`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36cb26c992a114bd50224b9eea9b3fabef4528c8ac1b1491b05d4d6a1886ea9`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e679549c9b0594b5dc1323db3cde02472a4fa2cc4dbcfad2f3925034f8e62`  
		Last Modified: Tue, 31 Aug 2021 05:06:36 GMT  
		Size: 76.1 MB (76133180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec1e759c05a811f810316f756889904a777305840694dbce8d41616fffb2e66`  
		Last Modified: Tue, 31 Aug 2021 05:06:28 GMT  
		Size: 32.7 MB (32735199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c41e2713c687f7c56f2f408e1063cd8756038afc615615f4238b2c28aa2667`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c8524cea13cd0d60ab079d11f926b595139ae0f1b8a6ca8e78fc386fd4683ecc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314037710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23ba52270226f4808eb5db842151fb54102254f2f869045e283b3d00cba56c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Aug 2021 02:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:56 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:40:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:40:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:41:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:41:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:42:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:42:02 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:42:02 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Aug 2021 02:42:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:43 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac2567afd7f21270eaf5dac9596df45b6dda0b77d64188744a7081a5f346b5`  
		Last Modified: Tue, 31 Aug 2021 02:55:58 GMT  
		Size: 104.2 MB (104162618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0daf045c79605e6b79149e30817a2a6a12ee94bd746d4ddbf97b159b86d9f`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053652fdf77cf09c2d5f748e1392a941b0a2640722c2e70d661cb0f79ed668cf`  
		Last Modified: Tue, 31 Aug 2021 02:56:20 GMT  
		Size: 65.2 MB (65183560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedc85ca67006659dbfc2b17452494645c1f0e417864446282ae6f592dc634e`  
		Last Modified: Tue, 31 Aug 2021 02:56:10 GMT  
		Size: 240.5 KB (240543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf81879f4a40b97c2359dafad0f780449e33d1663620a7c84e6edc1d195e3e4`  
		Last Modified: Tue, 31 Aug 2021 02:56:09 GMT  
		Size: 2.0 KB (2024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68fc5fc59c2a35f0a91dba364f8820a1bdf634a40ffa0598d351cb20b4af65a`  
		Last Modified: Tue, 31 Aug 2021 02:56:11 GMT  
		Size: 9.3 MB (9298963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3283cc3a3d0b05c08fbf8f9dd92a0d58882e3d3f4b30ad40605ca33f18330`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3042d28ddb6bf62c8b0e1e54bc0d10a513a2f5c9b3a1f4202288198c324738d`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c80802dfb985bc5e968ed325b0300ccc446bdd9de54b7af679333b9ebc11c74`  
		Last Modified: Tue, 31 Aug 2021 02:56:55 GMT  
		Size: 76.2 MB (76167513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d418353022c19184ddb5003057db95c611277d1f1bf4d789fab26eea7b08d5`  
		Last Modified: Tue, 31 Aug 2021 02:56:44 GMT  
		Size: 25.1 MB (25109980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1457cde4b44826bb5c7364ac964c0eea2aa3fb528fc1a5a935aec01b6be8bcf`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
