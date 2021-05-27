## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:0b8fd640b46e4a45e9a10fe4668c35d800d38118482a7cfdf70e0742b3ee6466
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:8200568e43742d60aa118d08ede4ee392a2b0f13dae087119e74fa4c942a0f48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300349890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71ae2761e0da5e96478db23ac877e3f3d98146d73da205e5717436ff7419794`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:14:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:14:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 May 2021 17:14:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 May 2021 17:14:48 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 17:14:49 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 May 2021 17:14:49 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 May 2021 17:15:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:16:00 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 12 May 2021 17:16:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 May 2021 17:16:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a04ce26341db0d6591d2793ca267552485c51f4cbb273019ac821d671266ce`  
		Last Modified: Wed, 12 May 2021 17:24:25 GMT  
		Size: 10.9 MB (10891745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad660b1585da7e0367ce63f17fafc6908ff07cb37a86a990231df068909dced`  
		Last Modified: Wed, 12 May 2021 17:24:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c6dde1ade4b0aa9d209f722a79ece3f88a0e7fecdbcd0c233656fc47e4ef53`  
		Last Modified: Wed, 12 May 2021 17:24:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf712e517ccc21a01aacc8ab5654a6fac578b379c312ebc3ab51765cf9331da`  
		Last Modified: Wed, 12 May 2021 17:25:00 GMT  
		Size: 239.0 MB (239023064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65e290ea31d62ef896514aeb7f8713ec481fae9a7bc2545d8d6fd5866a166d4`  
		Last Modified: Wed, 12 May 2021 17:24:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fd9f0669825a6b293bbc3a307b98db7251b478b0f16b3f39fc99e9a513df96f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244369399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e348486a2cc7b63271617129a7c7f2000374f16fa6b26d07d922d91a71ca1b2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:50:48 GMT
ADD file:ff9983cd659b3fc32ddfbbdeda76a971afd7d399e6d8b98faea3a9ead0e598f6 in / 
# Wed, 12 May 2021 00:50:52 GMT
CMD ["bash"]
# Thu, 27 May 2021 15:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:14:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 27 May 2021 15:14:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 27 May 2021 15:14:11 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 15:14:11 GMT
ENV LC_ALL=C.UTF-8
# Thu, 27 May 2021 15:14:11 GMT
ENV ROS_DISTRO=noetic
# Thu, 27 May 2021 15:15:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:15:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 27 May 2021 15:15:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 27 May 2021 15:15:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c54d9402d498e45ed396b5b6fe836f55e4ccadbad745decda3e9f83d880bc677`  
		Last Modified: Wed, 12 May 2021 01:01:40 GMT  
		Size: 49.2 MB (49225351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef41d27594cb3f96faef94886e77e8683347542ba8089a62b566c5cf3844f61`  
		Last Modified: Thu, 27 May 2021 15:46:15 GMT  
		Size: 10.9 MB (10883255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38226520a80dc952f0d3d4e18149770e870a41ae4a9f7b3a33978fff9ff5016`  
		Last Modified: Thu, 27 May 2021 15:46:13 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f353a3784dc41d355977847e3166eb4698d0a7de3cb8972e327419d596993bb`  
		Last Modified: Thu, 27 May 2021 15:46:13 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab49aa2abb9b66ea71c78a7bd5736c980ecb71c811ae93fefebdebed6b111a2`  
		Last Modified: Thu, 27 May 2021 15:46:57 GMT  
		Size: 184.3 MB (184258958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e891573a6d8e05da00ce9396f7343b16fd46d866f234cd2f411dc4bc74857e7d`  
		Last Modified: Thu, 27 May 2021 15:46:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
