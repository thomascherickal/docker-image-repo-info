## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:3818b7e8cb56bcc0f68e4116af42c0f8248a32806fbb10b0f1e67cf56eeea1a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c2b0941f8e1c25219f7cb728689141b38cb5d5b196eabf6401751e61fee9f762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235825969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e4a6abe543ff64330de8eace4054c64d3d530ae11d785990e54b1ceac7c1b9`
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
# Wed, 06 Apr 2022 02:36:12 GMT
ENV ROS_DISTRO=galactic
# Wed, 06 Apr 2022 02:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:36:56 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 06 Apr 2022 02:36:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 02:36:56 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 02:37:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:37:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 02:37:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 06 Apr 2022 02:37:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:3c59f0a65f8fb114421624ffcc95f4c2e75bb7fae35e3038cac0685e8636fbb2`  
		Last Modified: Wed, 06 Apr 2022 02:50:20 GMT  
		Size: 103.7 MB (103670028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72990dee2db5581c543cebde163f9a37e9a19ed0bd804a51ccd1637c56339d`  
		Last Modified: Wed, 06 Apr 2022 02:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf2abf969095f153378847fa209a5ed0a325ebee22d7fa1ecee8e342d57f122`  
		Last Modified: Wed, 06 Apr 2022 02:50:41 GMT  
		Size: 74.5 MB (74484144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42783508f954f832d8756f6cb3429facf0b286e7c10a1d646aa26ee5eee03666`  
		Last Modified: Wed, 06 Apr 2022 02:50:30 GMT  
		Size: 260.4 KB (260423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ef81da0ff8324493f2d8bbe56aa3e456a090d2e6871c8a0aa06b102683fde1`  
		Last Modified: Wed, 06 Apr 2022 02:50:30 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099c132b8a6d757e7ff1d6108abff83690c087fdc87ce483c52f527491e1c6`  
		Last Modified: Wed, 06 Apr 2022 02:50:34 GMT  
		Size: 22.1 MB (22113069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3efb115b0d98948a221cc14e2ff7c840921e79ccbcc69a9b4038c57c3fdfc866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224023179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df6227abc5427096e43808257d6679e239014354871217fedd16af2c2f9689c5`
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
# Wed, 06 Apr 2022 00:15:39 GMT
ENV ROS_DISTRO=galactic
# Wed, 06 Apr 2022 00:16:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:16:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 06 Apr 2022 00:16:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 00:16:29 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:17:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:17:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 00:17:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 06 Apr 2022 00:17:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f0a5873688a5a0d1f7a4a073085b0b55b579cb13f05009d03ce1a8d8bbbd77e8`  
		Last Modified: Wed, 06 Apr 2022 00:29:12 GMT  
		Size: 100.0 MB (100046108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21152fba7f49fee50b2482280764077a773a9ba1d5bb564367212ba4ea34af36`  
		Last Modified: Wed, 06 Apr 2022 00:28:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3317df3a918e61a730a1c4ee437205e30627aab9d04e3aceee62dd62fa9d46`  
		Last Modified: Wed, 06 Apr 2022 00:29:34 GMT  
		Size: 68.6 MB (68604421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c6b24fbdb482902fd7c6732b6f4e03c3b597b203aef61cff68fe4fe847597d`  
		Last Modified: Wed, 06 Apr 2022 00:29:24 GMT  
		Size: 260.4 KB (260384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f309095ecf7c1d12d36ca445418d9ad7bdd3db84b490c769ab5df5d5fee77c3`  
		Last Modified: Wed, 06 Apr 2022 00:29:24 GMT  
		Size: 2.1 KB (2137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73e5143ba84cf6b54b4f0ce46d90fcf2a7b8e045bcfaa8f7a6954eb70afce5b`  
		Last Modified: Wed, 06 Apr 2022 00:29:27 GMT  
		Size: 21.4 MB (21434612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
