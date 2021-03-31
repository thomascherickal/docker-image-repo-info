## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:1aee0a59abd2815192e3b2b82214ce19edaf663840504e40cbb2a040d65225a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:80788ee239491eeb65f5a4a2624d9970181658a205b66837aa86dac6672270e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322320701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed13e1a87f554706f5d42256847d5fbea833cd9d5ab23dcce0a0765fdc12b324`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:12:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:12:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 27 Mar 2021 09:12:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 27 Mar 2021 09:12:24 GMT
ENV LANG=C.UTF-8
# Sat, 27 Mar 2021 09:12:25 GMT
ENV LC_ALL=C.UTF-8
# Sat, 27 Mar 2021 09:12:25 GMT
ENV ROS_DISTRO=melodic
# Sat, 27 Mar 2021 09:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:14:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 27 Mar 2021 09:14:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 27 Mar 2021 09:14:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d657504ffb8f628d70a2b1e2672e16b95f6eac895057e4cdcb97e09f862a1b09`  
		Last Modified: Sat, 27 Mar 2021 09:26:42 GMT  
		Size: 6.9 MB (6869187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa6cca370d6196ae385348a9369c89f41ffa9578e97dddffed55be61d6e0e62`  
		Last Modified: Sat, 27 Mar 2021 09:26:41 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404a516aba8bbb9ba24fdc7ef19705ce8dd84915cf4cd2986249f95c22db251`  
		Last Modified: Sat, 27 Mar 2021 09:26:41 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb5474c655269c720249df5c38af05416a1d5e3d33019bffbcd827297ddd6c6`  
		Last Modified: Sat, 27 Mar 2021 09:27:27 GMT  
		Size: 270.1 MB (270070182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab44e97519ff7d9f42f3b133c7e261108a040df6ade9b5001b98fe56d831b1c2`  
		Last Modified: Sat, 27 Mar 2021 09:26:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:39f2688b7350d8777ce939b4a088a9b633a467ad0701be096124a410e2f54840
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274737083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e6130c2445162eb8e7e3f096081bcd1d3d35eab47497f4b66dd9d5ce112980`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:38:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:38:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 31 Mar 2021 13:38:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 31 Mar 2021 13:38:12 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 13:38:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 31 Mar 2021 13:38:14 GMT
ENV ROS_DISTRO=melodic
# Wed, 31 Mar 2021 13:41:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:41:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 31 Mar 2021 13:41:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 31 Mar 2021 13:41:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9bcb4567c53b5710817f63af7d0c14a3dad36b823f3cc9f142434d89dd7cea`  
		Last Modified: Wed, 31 Mar 2021 14:03:12 GMT  
		Size: 6.4 MB (6442935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84574c97c15ff3c495faceaf91ec7efac2d7735c4fe357cc256339c4fe93410a`  
		Last Modified: Wed, 31 Mar 2021 14:03:09 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefd0949cc578f2b84114a09843d05b951725916a271d79c9e803a14021734f8`  
		Last Modified: Wed, 31 Mar 2021 14:03:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fafb8ecac1b3a711771dfd44718d41e04b5dcf0e3545af1cc8fc71a84905bb3`  
		Last Modified: Wed, 31 Mar 2021 14:05:04 GMT  
		Size: 225.1 MB (225114741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e8c7efe0eb7db52b3a500557e94b2126eb204eaf0deb2cb3356cdd72b378f2`  
		Last Modified: Wed, 31 Mar 2021 14:03:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
