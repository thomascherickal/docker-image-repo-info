## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:1739d11f497daa23ef809bf15a68e4dde88f9220c365542bd68f0fb15287d82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:a5ee6b09e67675352aa10d5834871da5d23cfaf03a0b3a610716750b9535d036
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138966131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b62a87ff33315ca582301dc8d0913987d6db4216fe3fa681d099fce46aba284`
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

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:164fb6d4bcb478251a40a1bebdb398dcecb7cd646a8bb228a8d8374f55d09e58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2117617e0df8e25c1f2251e2de28e4d144e3cab050f5a03adad1c12cc7294175`
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
