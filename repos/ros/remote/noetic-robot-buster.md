## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:cae9e7165644a5521e437327c8215214192b32dff2d9424855634df2951b7bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:8c789faf60bf684ba716b389c2c54547a831543f3eb2a1ad3db2e63eb1f385c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.1 MB (484118955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6821c8dde635154bf776765f921f340e9ff95ba45bbbf2b4a102e01732645b39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 19:24:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:24:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Oct 2020 19:24:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Oct 2020 19:24:03 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 19:24:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Oct 2020 19:24:04 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Oct 2020 19:25:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:25:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 13 Oct 2020 19:25:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Oct 2020 19:25:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 19:25:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:25:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 13 Oct 2020 19:26:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a3a13f4da8a989cd47e5141fdd6f9cd9de6e86ccc396db6a668ad032a3160`  
		Last Modified: Tue, 13 Oct 2020 19:36:04 GMT  
		Size: 10.9 MB (10889343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64390ddd28a581349979be4bea66a21751b2ec96485b72280d0c7af425fbb8c`  
		Last Modified: Tue, 13 Oct 2020 19:36:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caaf435d5f32518773b64abc379057bbd924c553cfeb58874f5b1315bfc735d`  
		Last Modified: Tue, 13 Oct 2020 19:36:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfcaa897657f532536be04cfe0020d87bf81257a618757661653ce5441d295`  
		Last Modified: Tue, 13 Oct 2020 19:37:01 GMT  
		Size: 238.9 MB (238865739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14a3cb8bc6bc5df16b3677390c9b4780ea98a150b28e461422e141dbd5323b3`  
		Last Modified: Tue, 13 Oct 2020 19:36:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10751931502218188347b32494cacb109998b797c31081a9c99eac57d9c52da3`  
		Last Modified: Tue, 13 Oct 2020 19:38:34 GMT  
		Size: 86.6 MB (86562665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30482bd4183c03270a07fd2049f64776fce3ddebf54010a29379ff573d417dc`  
		Last Modified: Tue, 13 Oct 2020 19:37:10 GMT  
		Size: 232.5 KB (232476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edca43a1ddc44fc6a1f726452f297fa8c8c8b9029467fd689383dcc58ae4d0a`  
		Last Modified: Tue, 13 Oct 2020 19:37:26 GMT  
		Size: 76.0 MB (75966171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6af23ee1c7b439ccdbd465e3a347ddab2c9bd1f13b51decd66fb30ea8e834b4`  
		Last Modified: Tue, 13 Oct 2020 19:38:48 GMT  
		Size: 21.2 MB (21204748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4ac6426a8bbc20b0fa955ac36755f71daea40e9f11ddea29cf2a65c8adfad76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.7 MB (423682213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcd1c1909b6f5e08ce4abf729bc32c2592cab08eacd27c40e6feaa54baa21b9e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 20:39:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:40:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Oct 2020 20:40:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Oct 2020 20:40:45 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 20:40:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Oct 2020 20:40:53 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Oct 2020 20:44:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:44:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 13 Oct 2020 20:44:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Oct 2020 20:44:18 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 20:45:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:45:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 13 Oct 2020 20:46:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:47:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ffa15211d55c8de67be0d0ced3bbec2336b0250efc1e38a00b49df2b3ca22`  
		Last Modified: Tue, 13 Oct 2020 21:00:55 GMT  
		Size: 10.9 MB (10882041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946d470d5c44bd77a586608e501b75657edddef399cabbb3b784037a5b30de2c`  
		Last Modified: Tue, 13 Oct 2020 21:00:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3205eabe0fbcd56ebf5a0d111a79503bb9a68092500f018f21554bc69641b98e`  
		Last Modified: Tue, 13 Oct 2020 21:00:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a906801c61f426e1a99ed331e1f441f0731e34dee11c02124ef4c13b064b5c6`  
		Last Modified: Tue, 13 Oct 2020 21:01:56 GMT  
		Size: 184.1 MB (184094486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf60393679da03ef4644f7a560d3c43ca63dff47c5284f32bca35f7b2d7f4d`  
		Last Modified: Tue, 13 Oct 2020 21:00:52 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b04763c21890d355e7bd5801d806c3f0b9028c461cca195814580f40f7b96f`  
		Last Modified: Tue, 13 Oct 2020 21:02:27 GMT  
		Size: 84.4 MB (84355265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db545d99d11a6f3305b890a8e2edb0270ef30452387e403f6740a115ac9e28`  
		Last Modified: Tue, 13 Oct 2020 21:02:08 GMT  
		Size: 232.5 KB (232529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa6cdb30e141ac49dbdd6f9376003b6b8b9652bd332c2c67c1f4b8e5da3a087`  
		Last Modified: Tue, 13 Oct 2020 21:02:27 GMT  
		Size: 74.1 MB (74088490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac3adacc96da4c49fc93447ef33d10afd535052c19856c725d3738181959566`  
		Last Modified: Tue, 13 Oct 2020 21:02:44 GMT  
		Size: 20.9 MB (20852160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
