## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:ea9a012c0b385ac0628e08d718ce5ce20a2461498f0c7e17176751af1cad94f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:9256f2c0f5a77aff141a77cf1693d2cced0a5cd46667a98fac241c6c0f121767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.4 MB (349361641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219c699333392e98d64c806ce7a5211126915cbdf4eda09f9a0da0a96c7cba77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:29:26 GMT
RUN echo "deb http://snapshots.ros.org/foxy/final/ubuntu focal main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 27 Jun 2023 01:29:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 27 Jun 2023 01:29:28 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jun 2023 01:29:28 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jun 2023 01:29:28 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jun 2023 01:31:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:31:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 27 Jun 2023 01:31:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jun 2023 01:31:34 GMT
CMD ["bash"]
# Tue, 27 Jun 2023 01:32:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:32:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jun 2023 01:32:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jun 2023 01:33:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:33:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jun 2023 01:33:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jun 2023 01:33:45 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jun 2023 01:33:45 GMT
ENV ROS2_DISTRO=foxy
# Tue, 27 Jun 2023 01:35:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.7-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:35:30 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74a3b07252b944b4ea5463c9fdd65f55bd7b46d44ca3316395ba9bf84c0a427`  
		Last Modified: Tue, 27 Jun 2023 01:38:49 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20eb6b1e59f8d211aded68a06cfa5675f43f3fd0db8c28eca135aa6150228079`  
		Last Modified: Tue, 27 Jun 2023 01:38:49 GMT  
		Size: 3.2 KB (3217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d888ae97575093a5fa68bf21033f4f40fcba809edb8d0be31d93adf559a990`  
		Last Modified: Tue, 27 Jun 2023 01:39:08 GMT  
		Size: 120.4 MB (120424933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a47a9caf44acbe4edf6fd3f71ae01efc21add261266da6cc6f5e2f520428c3`  
		Last Modified: Tue, 27 Jun 2023 01:38:49 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7e8c04c766471734e7b28ed1b76ecc23cb788e674764853e0ee71244ce7b52`  
		Last Modified: Tue, 27 Jun 2023 01:39:27 GMT  
		Size: 73.5 MB (73507288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae845ad132a5dfb24be6ecd01d9223d39adf2c844effaccad994dd0e6370168`  
		Last Modified: Tue, 27 Jun 2023 01:39:17 GMT  
		Size: 264.9 KB (264879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459004dc4722ae66298bcfed7d63d39426386f62cfd25fad5d68bd1574ffe157`  
		Last Modified: Tue, 27 Jun 2023 01:39:17 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcaec1daf5e724808e7de45067614a1f6262ae1896aefc0f3c2a1c30bd1c00e`  
		Last Modified: Tue, 27 Jun 2023 01:39:20 GMT  
		Size: 21.7 MB (21677105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8009dc976f6da5e4703ad0e5cd3363fab82d8921f935c4e84533f020c82af72`  
		Last Modified: Tue, 27 Jun 2023 01:39:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f4bbf3025363904cb24a3c22c9430e56c2f14dd3abac8e1ac338dde13ed615`  
		Last Modified: Tue, 27 Jun 2023 01:39:37 GMT  
		Size: 5.0 KB (4993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef01520b525e0f093e513e4de377abc833e03298733f7c79e74abecf0fb1f11`  
		Last Modified: Tue, 27 Jun 2023 01:39:50 GMT  
		Size: 76.5 MB (76450865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633ae1bc651389d6a9bb8e88a03cffa1edfc23f1ed8cedf5ab6c845aeaba7008`  
		Last Modified: Tue, 27 Jun 2023 01:39:41 GMT  
		Size: 21.7 MB (21691985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f01db679211c1506dd49aad892c81ee4b10fb7ce06350a1b4e2e3329ff06b3`  
		Last Modified: Tue, 27 Jun 2023 01:39:37 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5e47961327cb3a99db8f9906a25bf84b92493c3d132ff6029b0386882173b612
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (317970958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a1e11bd6404bb9dcd240f44fbf23f0d92846b02ba0fa7ee4d40bda7251e1d4e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:23:57 GMT
RUN echo "deb http://snapshots.ros.org/foxy/final/ubuntu focal main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 27 Jun 2023 02:23:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 27 Jun 2023 02:23:59 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jun 2023 02:23:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jun 2023 02:23:59 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jun 2023 02:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:26:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 27 Jun 2023 02:26:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jun 2023 02:26:31 GMT
CMD ["bash"]
# Tue, 27 Jun 2023 02:27:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:27:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jun 2023 02:27:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jun 2023 02:28:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:28:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jun 2023 02:28:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jun 2023 02:28:59 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jun 2023 02:28:59 GMT
ENV ROS2_DISTRO=foxy
# Tue, 27 Jun 2023 02:30:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:31:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.7-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:31:03 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034efe4678b833917f300002fb3d3f08d1067cbd8079e778a59f27dbe1f6294`  
		Last Modified: Tue, 27 Jun 2023 02:33:37 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d0d2f4682fb4720d5bf2479d8416b51c5035a34376e6c04d6b9aa67e5920d0`  
		Last Modified: Tue, 27 Jun 2023 02:33:37 GMT  
		Size: 3.2 KB (3215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539183fce8753ce3d5d8c51fefb7241ab37e38ef3035a0f06c4cdf69df0df48`  
		Last Modified: Tue, 27 Jun 2023 02:33:49 GMT  
		Size: 104.6 MB (104637136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00986e50155632a9acd124b403b5f90a825cc64328f167d8e745845e56a4731`  
		Last Modified: Tue, 27 Jun 2023 02:33:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdeaaf97feaf549335ec896afd139bfe09b4297e72657d1b379f7feed781ce2`  
		Last Modified: Tue, 27 Jun 2023 02:34:05 GMT  
		Size: 67.9 MB (67871739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ba3d2091202e58c3a62003469a0376df766f94286790a2b295c11481d225a`  
		Last Modified: Tue, 27 Jun 2023 02:33:58 GMT  
		Size: 264.9 KB (264869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec731a55426958a0ad6c6cd34dc9ca403f7b057835c68ac93674fafedd59b68`  
		Last Modified: Tue, 27 Jun 2023 02:33:58 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4171f6d5d1e47b702217521799c4c1aa90e1f8b1e5b35bb4ffeb8ee178284b`  
		Last Modified: Tue, 27 Jun 2023 02:34:00 GMT  
		Size: 20.4 MB (20404964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9695ce27e3aa0455b05dcb9b6e3a3a56d23434ae602430a03b9b4832a5ae948a`  
		Last Modified: Tue, 27 Jun 2023 02:34:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d67704ba806cf7fd45098560bc3eb0aee78b4383f79c73a153ec40c1cd54a43`  
		Last Modified: Tue, 27 Jun 2023 02:34:15 GMT  
		Size: 5.0 KB (4992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6900dc4b2ce805af4a5782182fd215d72f1013aed54d2ac924278a77aa15da`  
		Last Modified: Tue, 27 Jun 2023 02:34:26 GMT  
		Size: 76.5 MB (76514119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ba0e4e346e952e904686c0f7b6f615e62cdfc933277396da7436f91ff35e2`  
		Last Modified: Tue, 27 Jun 2023 02:34:17 GMT  
		Size: 14.3 MB (14332857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb62be6aa3f3b6f06f433cbfa1ed6fcf1d6933044876b16b0430ad99a2d649c`  
		Last Modified: Tue, 27 Jun 2023 02:34:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
