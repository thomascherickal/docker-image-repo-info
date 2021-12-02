## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:cff0b5a0c4fe48adfef7d0bd02eb4009e56a932541c71fca9c4ec7bf397cb5d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:1cfa864fcdb3733b854fcb2bc2d474a1727099f22e78fd57b90fad7130b52db6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300418498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:480154696b7d95f4e24afb577c43ef157189e425d7b5c53d6563ebe1c6c060f8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 22:36:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:36:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Nov 2021 22:36:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Nov 2021 22:36:28 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Nov 2021 22:36:29 GMT
ENV ROS_DISTRO=noetic
# Wed, 17 Nov 2021 22:37:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:37:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Nov 2021 22:37:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Nov 2021 22:37:37 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f64a2cee9a8973db7ffaff43c62f68f0db43144b718c8339856ff2d039b430`  
		Last Modified: Wed, 17 Nov 2021 22:43:20 GMT  
		Size: 10.9 MB (10891910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d367fa9b39ce393432a2a974cff50cc6c0a295b0c00a6a71152b947621dfd2`  
		Last Modified: Wed, 17 Nov 2021 22:43:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54972089aecf2d558033d5c01eb20f1a2fc64c872aca23ad9ab78f45f335f6e4`  
		Last Modified: Wed, 17 Nov 2021 22:43:18 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d68c1a3d9a31ff02e5ed0caf544e9e047643eeaa48073c11c2aff158e93739`  
		Last Modified: Wed, 17 Nov 2021 22:43:56 GMT  
		Size: 239.1 MB (239087074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb488c1f6198579f8b779a8d04bba2ad192ec739f12e0996b08295f67e238be`  
		Last Modified: Wed, 17 Nov 2021 22:43:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a8fb3f5cd851acbd8709afda777515f2333c9ccb3fb689176b71bcf1d1a38551
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244215029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fcc8d12e363caeadad4015fdfa946ab9074370766cdc836909e980add4fe3d0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:09:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:09:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Dec 2021 14:09:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Dec 2021 14:09:49 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 14:09:50 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Dec 2021 14:09:51 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Dec 2021 14:10:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:10:56 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 02 Dec 2021 14:10:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Dec 2021 14:10:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e8f1f129dad6b169099626334d47f33bb82f4b4bb0546404f0e3ff9f29f589`  
		Last Modified: Thu, 02 Dec 2021 14:18:09 GMT  
		Size: 10.7 MB (10688015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a995ef6e0affa0efea1e9bab7ccb010f6b50dc0dd518f955224c42c80ca4625`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1a144f0e750af7280088604a588b33ca097d137deb1e9c165832bcc112ff12`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ff02a2b334915606915d72debb67ed7feaef6ab150ded7a474ed2a3847bab`  
		Last Modified: Thu, 02 Dec 2021 14:18:39 GMT  
		Size: 184.3 MB (184301599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4546300f0a7a750dcd6fdf3c875bbd66d4444983e525a6fab1105911104a496`  
		Last Modified: Thu, 02 Dec 2021 14:18:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
