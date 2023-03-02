## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:c291a518efe3612ab93be991d138def5bd20352502cc87a059a28d8b48fba979
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:cfc9335331d64eb79d9995454f6f4dbb6a812882ce6f31621b06a3537bc20233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349022665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7dcec79d7a96ec6a3187b2ca0c148ba865355d2049885b82ef8f0377cd7e32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:45:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:39:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:51:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 20:51:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 20:51:46 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 20:51:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 20:51:46 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 20:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:52:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 20:52:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 20:52:50 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 20:53:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:53:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 20:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 20:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:53:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 20:53:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 20:53:53 GMT
ENV ROS1_DISTRO=noetic
# Wed, 01 Feb 2023 20:53:53 GMT
ENV ROS2_DISTRO=foxy
# Wed, 01 Feb 2023 20:54:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:54:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:54:32 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db143da9f5a088b47cfbe87905f9e615f3b537f906257fc11ac7a38ffb0f236c`  
		Last Modified: Wed, 01 Feb 2023 18:58:42 GMT  
		Size: 1.2 MB (1154526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52bb4834a5fa25fa5b39cba579b1676bc6fc585a61819ffad44865e1f80e40`  
		Last Modified: Wed, 01 Feb 2023 20:55:33 GMT  
		Size: 5.6 MB (5553686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f105b35b0dfc6028b74d92fda44d6d2c3af732aca846352b68466fa262457ea`  
		Last Modified: Wed, 01 Feb 2023 20:58:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da6af1c9709b569597a5ba230c17042bc010f9750727f5c8758e5b1772139b`  
		Last Modified: Wed, 01 Feb 2023 20:58:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390ba395fc8695bc2fa5c6b394cd5d5646325ef60302c849898873530f6d9b1`  
		Last Modified: Wed, 01 Feb 2023 20:58:29 GMT  
		Size: 120.4 MB (120357173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c508771ef6bc75da73349529405df86553b5351d4963f8b9a0f9b0bd39b568a`  
		Last Modified: Wed, 01 Feb 2023 20:58:08 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04699b3e750a87a1ac026108652f71ed30dbd1658b8992675307ee50b00d13bc`  
		Last Modified: Wed, 01 Feb 2023 20:58:47 GMT  
		Size: 73.3 MB (73334255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60655459143d2e28fcf98e47908a7e7521455039a65dffdcde118686599dc91`  
		Last Modified: Wed, 01 Feb 2023 20:58:37 GMT  
		Size: 277.8 KB (277775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ea369debb9602b8c58eb54bc2ae097a85dca159d27e70505ae0b6dbfb73e22`  
		Last Modified: Wed, 01 Feb 2023 20:58:37 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c16f94d4b42426319c336c992c2ae0a9420d2cda68e8de9c663e7544512d8d`  
		Last Modified: Wed, 01 Feb 2023 20:58:40 GMT  
		Size: 21.7 MB (21662340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46476122dd2038ad522fb84e072fba616b953e8bfe5a3fa3f2e323891f03f2bf`  
		Last Modified: Wed, 01 Feb 2023 20:58:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe415d2ec986c55268b230b5b29c45041788ff7ac04826df3945470bf5838547`  
		Last Modified: Wed, 01 Feb 2023 20:58:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74e3379ac16a555e64ef871a2c5651b863633d9cb95ff85d7576ecfd0cc57de`  
		Last Modified: Wed, 01 Feb 2023 20:59:13 GMT  
		Size: 76.4 MB (76425373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5f548ac31300e2ac3f13d7ff94a0a602954b0d370cfecfe4d7ae3dbc80380d`  
		Last Modified: Wed, 01 Feb 2023 20:59:03 GMT  
		Size: 21.7 MB (21674188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed68eac63e4eb76c7c609c7830803226e12948e7a9acab40d56e0c6c0fbe4b75`  
		Last Modified: Wed, 01 Feb 2023 20:58:58 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a0b3325105eac515d5465568286afdbf4bb402bc1ee5bc35a01dba6131fd441
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317620039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fec20d33a0e5320521134c4dd19ad08b2c7c9cafc4779108e04e28f8604277`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:45:23 GMT
ENV ROS1_DISTRO=noetic
# Thu, 02 Mar 2023 03:45:23 GMT
ENV ROS2_DISTRO=foxy
# Thu, 02 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:53 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57336bd1f5b659fca7d2c15f05835498bece96470d7126cb8c6994cc661da08`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d551c2118ed584d3c3117d35f5f86852fb5428cf57422b5cdfaad1a12377f5`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d997e889567155d577278109c067af17322ca8eb3c71a7488070d6a4948495c`  
		Last Modified: Thu, 02 Mar 2023 04:09:47 GMT  
		Size: 76.5 MB (76491880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82b2ada8d839cd2b72c7f974a2d7323f582f2cf836821c1678dacf155bb5ac`  
		Last Modified: Thu, 02 Mar 2023 04:09:38 GMT  
		Size: 14.3 MB (14325041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e355150cb1e9732212022cc89c7a129d8d79a62013c5570671e3a2166ad888`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
