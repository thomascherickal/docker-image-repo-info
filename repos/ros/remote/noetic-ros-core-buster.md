## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:2909b34c7b1c64431ca0f75bec7eda0857c4815c58da9e62d4858e2973582a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:1a1d06b35677ea6f17b411b6bcb701c371187b5cde9933440638403a1a3f3a33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300522668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0366cedccb9e45dc41095871119e8aebed346194dab88db7bd95ba5f71e98c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:10:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:10:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:10:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:11:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:11:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:11:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91dd5198cc577c5556c7c5c335e0ea5701168d8c2ded40b83bc24be1434e47`  
		Last Modified: Tue, 23 Aug 2022 11:17:01 GMT  
		Size: 10.9 MB (10893537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385a586942561cc66fbd30195e87e96f1b39c6350f5ecd935dab71ef933e1bca`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3402e2486e536bf44469c2ce583b71937b7cbff76618e426dd63ed6b7dfe0cc5`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c2873f607da18c9f2623d952abd04118f7d0778f3599821850f1919eafc164`  
		Last Modified: Tue, 23 Aug 2022 11:17:33 GMT  
		Size: 239.2 MB (239186445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17c4e21a19faebaa430ee698b7cb100d2e778f790784743bdc70da09436a41`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b8a2f95e3a3e173aaa2bb444bccdca8fc2e86c556b35596b039e7fccbbe9633b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244293507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89673ed8d38d107a06ec46cc1af47c271e78a4301bd71e7e62fcfa10850e23fb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:18:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:18:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:18:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:18:57 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:18:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:18:59 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:20:21 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:20:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:20:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc5b8055a31acea8cf6858fb7058f9828cf856d7ca15408120754ef8e582e8b`  
		Last Modified: Tue, 23 Aug 2022 11:28:27 GMT  
		Size: 10.7 MB (10689268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3e051ec8c4f50bc9206c4036995d09b8baf8a208b4aae22a2deeb7a246a5f0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3dbf6ff20222664e13d9f371430b5b76a850b135d2cd6876f8239ebf2cf26`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6b972b9d90022d411ed9be6a75b03629caf11045e410b85bf532d9b574973f`  
		Last Modified: Tue, 23 Aug 2022 11:28:56 GMT  
		Size: 184.4 MB (184373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bebe4a80f1367e9d727dcccb4679e5590d80dd2a8d0b00100b06f21a5e20bc0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
