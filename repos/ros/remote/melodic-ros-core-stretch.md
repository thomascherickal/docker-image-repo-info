## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:3de3fcc355472e813f870eaa1b324b9b6e71407bcb3c4db9e19dcf2bf5e2ce86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:e58e45593a082bf6ad7432f40ba5bab14e11d6d2c430275e1cd2db3fcb2a2c14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322295226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ad8ccaad1925d06a6124d04d7fa20e463f3fa7b995a81fc8597ccb328a4ea5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:09:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:09:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 May 2021 17:09:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 May 2021 17:09:16 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 17:09:17 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 May 2021 17:09:17 GMT
ENV ROS_DISTRO=melodic
# Wed, 12 May 2021 17:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 12 May 2021 17:10:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 May 2021 17:10:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a867e9d598a219f826e3b76f5280f3d106205d5fa6b8e1f2d421fd463d8fbc`  
		Last Modified: Wed, 12 May 2021 17:21:34 GMT  
		Size: 6.9 MB (6869206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302212f98ddaf07466a1b811fe425f01ff9f85b2778ce2d5b97611934d34240f`  
		Last Modified: Wed, 12 May 2021 17:21:33 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b35ff6673ef12169b553429937e2fe4a366a68e6eb03770829a0b95f3361ad`  
		Last Modified: Wed, 12 May 2021 17:21:34 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70bec3846c6a4887618d8cf19d2db025d8d2122df811164567153330bf2e1a8`  
		Last Modified: Wed, 12 May 2021 17:22:22 GMT  
		Size: 270.0 MB (270044121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0faf0f68b02c8fbcd34133d9f9b4bc1413a3f0851320b60e97d7f30e2404b931`  
		Last Modified: Wed, 12 May 2021 17:21:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f6d4294164418e1e747c77c841e065d8e78c13a438a7d8a2ac983faaeed3d985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274739255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:836a904b0fca51cd368b114e3e09d60da1b9a01ad1dc6a7fd3d649c8bc9e44c1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Thu, 27 May 2021 15:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:04:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 27 May 2021 15:04:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 27 May 2021 15:04:57 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 15:04:57 GMT
ENV LC_ALL=C.UTF-8
# Thu, 27 May 2021 15:04:57 GMT
ENV ROS_DISTRO=melodic
# Thu, 27 May 2021 15:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 27 May 2021 15:06:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 27 May 2021 15:06:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a98e1e3f21a423192b7c1a0497b1b7bfc382689c0aff9a0673c2497a89c2f9f`  
		Last Modified: Thu, 27 May 2021 15:40:04 GMT  
		Size: 6.4 MB (6442854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aec0a67d93178c66f703b46387890df2610467fc051d6d75bbeb69084cfe7f9`  
		Last Modified: Thu, 27 May 2021 15:40:04 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d81359b86841e869b88f3722c9d07b8bad9165ee109b14f0e019d09d7ec95f`  
		Last Modified: Thu, 27 May 2021 15:40:03 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481a6394104cb7b757467168f40d8aac2412a1c4e71b6a60767c0254f15746e`  
		Last Modified: Thu, 27 May 2021 15:40:50 GMT  
		Size: 225.1 MB (225116762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8a806cbdcc74413856d83aae37a9b56f48ce5d4acec963f8b78155d9565ab`  
		Last Modified: Thu, 27 May 2021 15:40:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
