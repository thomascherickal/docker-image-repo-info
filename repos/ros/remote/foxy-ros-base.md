## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:57f2d75332720d1908001425525e2b02a1e34a8d578f1407560c98392f10e93e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:3d6215a670938f4440da44f4f81876751486045f30e53c378c1d0a184dfa17d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251864459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6f2ca0b19c406200237b0e7af5ed89bed24493991fd76d6555b677210c0aee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:50:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:22:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:33:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 06 Apr 2022 02:33:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 02:33:19 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 02:33:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 02:33:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 06 Apr 2022 02:34:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:34:16 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 06 Apr 2022 02:34:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 02:34:16 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 02:34:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:34:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 02:35:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 06 Apr 2022 02:35:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbdf8d1aa53ac931cb020f1ee4ae35afbc9afcf41aa966fed51bc2848d19d4c`  
		Last Modified: Wed, 06 Apr 2022 00:01:59 GMT  
		Size: 1.2 MB (1180816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbffaa3aa803be1d98256e0c9f979dfce3a93c8d4e1e03d457d43d5b26e4c06a`  
		Last Modified: Wed, 06 Apr 2022 02:45:59 GMT  
		Size: 5.5 MB (5546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d8b35ed8c1193d1c7632795e2e746af76665e053b6265bc3aa6fcdcc2f6ce`  
		Last Modified: Wed, 06 Apr 2022 02:48:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecde8263a7e151cd29ce7e15f1d2a3839c993a4e95a906bc3ea874e3a35a84`  
		Last Modified: Wed, 06 Apr 2022 02:48:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbf4df1bc05bf9e176c25612e7a8ec7b342effedb1dc1e2525648f7860034ea`  
		Last Modified: Wed, 06 Apr 2022 02:49:00 GMT  
		Size: 120.1 MB (120104166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee45a379c1a62a248c1d29cfa77cc083dc0aac1464d04d8032670c22daf969`  
		Last Modified: Wed, 06 Apr 2022 02:48:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f872d09bcfc860be4ac26eede5c719c244f5675d4d1c03864accc8665429003`  
		Last Modified: Wed, 06 Apr 2022 02:49:22 GMT  
		Size: 74.5 MB (74540381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762b9fdab6993b96776f4742c202419043905b6e63701d905bda1803ffdc781f`  
		Last Modified: Wed, 06 Apr 2022 02:49:11 GMT  
		Size: 252.9 KB (252877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f379d3e63ada63cdf7e7972823f8de0cfc1b16e1cd843a396db09b3ec26e9a2`  
		Last Modified: Wed, 06 Apr 2022 02:49:11 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966725d840727bdf64fa557ca9fba77ceccf04121c7ec7f8b69eb951c3968c02`  
		Last Modified: Wed, 06 Apr 2022 02:49:15 GMT  
		Size: 21.7 MB (21668752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ae36fae3e82c0d9f9c4e3258f44dd28e3877ac277a132e8976f087a85a63fdfb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227241332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce15724c4e91d0bfd625de643cf98fc6e82723e6be23b507480d6e311d1f01a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:07:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:07:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:12:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 06 Apr 2022 00:12:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 00:12:38 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 00:12:39 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 00:12:40 GMT
ENV ROS_DISTRO=foxy
# Wed, 06 Apr 2022 00:13:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:13:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 06 Apr 2022 00:13:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 00:13:31 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:14:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:14:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 00:14:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 06 Apr 2022 00:14:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a8b80bc3dfe754b09e8f3623fb3cd9e300bee4e2ee1ff5d754e921ff23e802`  
		Last Modified: Wed, 06 Apr 2022 00:24:48 GMT  
		Size: 1.2 MB (1181994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8cfeabbec8839214562f2254e216ef5cfc5a5809f29bc698db7732e32a1392`  
		Last Modified: Wed, 06 Apr 2022 00:24:46 GMT  
		Size: 5.3 MB (5321759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfd349c1b512e83e2c714c8d8970014c2507a69e63b807a3d8d37fbb3519482`  
		Last Modified: Wed, 06 Apr 2022 00:27:31 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1245930ee161c6386e5cfe90f972dc34e270479504f64232e6c4af62fa4cb`  
		Last Modified: Wed, 06 Apr 2022 00:27:31 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce55c115335a279fdefcc0c9fb85bd775f8c5efc5af6eebb6c9b636c7030038f`  
		Last Modified: Wed, 06 Apr 2022 00:27:48 GMT  
		Size: 104.3 MB (104275827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2e54b04b89c55b7c3a3d7a32ba20aee3380d359535d73d86c12127600cc02`  
		Last Modified: Wed, 06 Apr 2022 00:27:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a414235eacaa94106e31ab7b3a98138ebedaf7bd6daa5b580ab406aac5dbf8c8`  
		Last Modified: Wed, 06 Apr 2022 00:28:10 GMT  
		Size: 68.7 MB (68661871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc5f57fe07ccf949f06d61ba62ef81e02d3f55882bcfa4166b7bf9901790e91`  
		Last Modified: Wed, 06 Apr 2022 00:28:00 GMT  
		Size: 252.8 KB (252826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e6a570819989ecbcccd50477a938c4d58d928d1179d50584fe889b0b1f528`  
		Last Modified: Wed, 06 Apr 2022 00:28:00 GMT  
		Size: 2.2 KB (2157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55ce927f4a8086c903eb64847becb8281dab4acd480b3fcac7a1900ee54c8ee`  
		Last Modified: Wed, 06 Apr 2022 00:28:04 GMT  
		Size: 20.4 MB (20373134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
