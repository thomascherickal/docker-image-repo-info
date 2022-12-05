## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:b021f08c32cb3c162cce073bb5fcb0f150ab5caed221b4786791619964469bac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:bab22323a0214f5fa9cafb98e00fa71861f9c2d57b95aa087b2ef20eed7bbd43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330069416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5eb59b1f887e3059879623790ea7d4208917f30f8f460b74e07257048e2eb4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:31:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:31:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:31:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:31:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:31:37 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 07:31:37 GMT
ENV ROS2_DISTRO=galactic
# Mon, 05 Dec 2022 20:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:58:40 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7f5b5c701916838562eb61ea9d238d42ecdcf4603217d5f36de002d875373`  
		Last Modified: Tue, 25 Oct 2022 08:01:15 GMT  
		Size: 73.3 MB (73280543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dfb5edf358837c3acdfe4765a62b10a0588d5ee88a202f18c6decb245a6c4`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 279.6 KB (279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81213e1334be0f25c6545b79677786f9e06c1aaea8a510b21195f4dc08b6ecac`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c4d1072c5bb0b70378dd5a649ff6468e2763e77a087f95fa4e934dfa18632e`  
		Last Modified: Tue, 25 Oct 2022 08:01:06 GMT  
		Size: 22.1 MB (22138749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f8c44f31c8de7186a01b87fd4516c3397f99b9cd341f36f8cd884940d852be`  
		Last Modified: Tue, 25 Oct 2022 08:01:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08eb43ea9a6ec61bf6c97f1d126b6a349c84449712c18182f9bc67d4229193fe`  
		Last Modified: Tue, 25 Oct 2022 08:01:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee3bddad4ed426da9149f801e402c4e7b31092b050e28307f810faf15566d5d`  
		Last Modified: Mon, 05 Dec 2022 21:00:40 GMT  
		Size: 78.7 MB (78711799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52095e933e87e6b024c09ed3e6e8b75ed3ad78be4bb04827964a51d673b3d05b`  
		Last Modified: Mon, 05 Dec 2022 21:00:27 GMT  
		Size: 16.5 MB (16465249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658f01ec3401ce6e030e463e354d30073b745fc73a48c21d33f508e2b92e230c`  
		Last Modified: Mon, 05 Dec 2022 21:00:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:637e82c995b77e792f72678a04b606474c16d04a9b80573cde6172cd4399196e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318262296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d42d352759ead3aca27aa07fd7dbda028a70324f28e1c2d59b8b6b49315367`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:39:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:39:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:39:58 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 21:39:58 GMT
ENV ROS2_DISTRO=galactic
# Mon, 05 Dec 2022 21:30:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 21:30:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 21:30:40 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb15d0de8d57e94728781ae793ebb9c47da6af6d21a8a38c4506decc8066b63`  
		Last Modified: Tue, 25 Oct 2022 22:07:56 GMT  
		Size: 67.6 MB (67619873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7674f0c0caa8655a1368b99f006f9efd6c9309ac5fb7eb7aa609b2b0e9ceb`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 279.6 KB (279608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f136bdb9a4de4a69c2fd48d4558581abb495390dbb234332d4e4feecccbc78`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5041645cebe7017ddeab3344686c7feca135348dedf51a23c6c4595ba1d2e826`  
		Last Modified: Tue, 25 Oct 2022 22:07:51 GMT  
		Size: 21.5 MB (21475535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7a424e7ef0057fa34db63d0489365de499500ef3615cbd982ee78c0b4e674`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f618329feb5073887e7596cff8d8ad3752efb4da04ddb54e58b0b42f535cda`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae93c3b880aa3d7db0b5516f8dea5297976b8bb4dddd18a78332e91311e7521`  
		Last Modified: Mon, 05 Dec 2022 21:32:35 GMT  
		Size: 78.7 MB (78675979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136144faf407c9008ab1468dc80c1bfc0ebb3da3018a7580ff09d8388924f998`  
		Last Modified: Mon, 05 Dec 2022 21:32:26 GMT  
		Size: 16.0 MB (15988638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff1e5a2ba475ab10aafe8900f8f958719f5a5f878af891a2f26ea8dfe69b50`  
		Last Modified: Mon, 05 Dec 2022 21:32:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
