## `ros:galactic`

```console
$ docker pull ros@sha256:d0699e4ade0748bda3c9325cc821e27670dd4714a13ebe035cfe8d79a9c87cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:28ca84182f0ee87aca4d0f87192387544549540246bac34f56c34d2848fc6323
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232051568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a167de5fe893c22c072d577ac26b70b9b56edf708870f19f5ba6a7775875e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:24:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:25:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:25:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7965e0f107cc789a111cb3aa5eeccbd0301fed15c9b12b6ef20f7189fdcb19`  
		Last Modified: Wed, 14 Jul 2021 02:37:58 GMT  
		Size: 70.8 MB (70796695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6f6e6066357111dc70ca230ecf7ee7fc275ffb6d673b41ca24523aa05447`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 239.1 KB (239064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695aa247c643fba1c6637b4e18f867bff6915c0e30aeec58fb120791bf6eeeb`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ef9d4a7fb46254a46a0a519d9b72965918875f359d7528c7a0fc75c884477`  
		Last Modified: Wed, 14 Jul 2021 02:37:51 GMT  
		Size: 22.1 MB (22095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abc211eed9fdf36bd18f37531c639173ac8d34a937e7565fb52bfda545945916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220687765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0654be371efbe96156b89adf874e1665812be939aa6d7e21c3b8cc380913ff06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
