## `ros:humble-perception`

```console
$ docker pull ros@sha256:39828be6397f30e54b0629ec7df3d526f49d4af4276245afbec6ba265fb4c146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:5e5ea6fd504d3d0a45bd8c464e0d9da7c113d318d6ee9a346c8a1cd4fba7b8c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **953.6 MB (953584554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc9075856b7daa752a9aff6d139115ff9db78fe2cf98222c71740a1003e2697`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 01:34:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:34:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:34:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:34:32 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:35:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:35:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:35:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:43:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e66f33d318c436f08fd59b9535f8c20afbc41d9d7fe918d01784046bbde6c`  
		Last Modified: Sat, 02 Sep 2023 01:50:49 GMT  
		Size: 106.4 MB (106393782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941567335e5935ceef4278336eb962350c2dd265f6daec9c649f2229e64f67ca`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c4906d79a11eff8f78dcccd3c6d7ae490a0f02a581f3f3e96a6811b9afe08`  
		Last Modified: Sat, 02 Sep 2023 01:51:11 GMT  
		Size: 98.1 MB (98119987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bcf88c07168233fc1f6f6898e4db9da4b4059228dfd1e3e46d397186946e38`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 314.3 KB (314302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be25f77b8e406c44975f550fa8153ab4077501118853bb2332a5c1f532e8e5`  
		Last Modified: Sat, 02 Sep 2023 01:50:58 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e776a75381e899f2343f05d298944ff4ae87f06edf6090b6b69ecc5bc342863e`  
		Last Modified: Sat, 02 Sep 2023 01:51:02 GMT  
		Size: 23.1 MB (23089197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7bd313849f09cf70f1a2108141db6f7610dc479829316180863437ffc52a1`  
		Last Modified: Sat, 02 Sep 2023 01:52:52 GMT  
		Size: 690.2 MB (690181677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1012f29357f78f9bb00ce55bfc95072973d6ae73627674b5ef4837114001aa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **914.1 MB (914088422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2193a560c90e7968ca85465a319d367d990e8026e8a668ee951ee34c2da0fc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV ROS_DISTRO=humble
# Sat, 02 Sep 2023 00:25:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:25:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:25:07 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:25:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:25:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:25:45 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a295b8a66bcb3a64684c4c57388e4c53eb16e08c6388d1c528220854c1473c9`  
		Last Modified: Sat, 02 Sep 2023 00:43:20 GMT  
		Size: 104.1 MB (104123742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843c4bd601a8295db4d64a4af68d90f98ebf28ee9bc4831d0d8ef6900fc2e27b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450003932f122cef453b721c74a349ef5e6dee2503cfafdc5584691209809c19`  
		Last Modified: Sat, 02 Sep 2023 00:43:40 GMT  
		Size: 95.7 MB (95680017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ca121d14fe945dfc4c8138cbdfd144695d6634e53ecd9739b0a38280a10bb`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 314.3 KB (314295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba5301f57280a3b5523918a7706a4f75580c5c0d0f18fc694c055af5135216`  
		Last Modified: Sat, 02 Sep 2023 00:43:29 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9442090566b229f0b496eb3db50f6b3464c97769f46550dc5f4bc098e7a7f`  
		Last Modified: Sat, 02 Sep 2023 00:43:33 GMT  
		Size: 22.5 MB (22515200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8590d691e0846807c4802d8a4a74d60b6d0600c0a2d1cc6da88d0e6899e06d8`  
		Last Modified: Sat, 02 Sep 2023 00:45:14 GMT  
		Size: 658.0 MB (658038945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
