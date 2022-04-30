## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:0d03e74cfe94c9ef859bfa3833474469ae35a60ffbb567c186716bdfa855dbb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6712e4c2f61d50d9660d3cf17db86aaffc70f817a32640014c7d1581fa053330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138960524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08cc80d8fbbea164891e6a75216cd7e78fd4819948127e757f3159f8d5b1e5bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:39:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:00:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:11:21 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 02:11:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:11:22 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 02:11:22 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 02:14:07 GMT
ENV ROS_DISTRO=galactic
# Sat, 30 Apr 2022 02:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:14:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 02:14:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 02:14:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca43c78a9071a3a99b9aa1fe030cf8ba61c96fbf0b12adc1a85163d395cc10a1`  
		Last Modified: Sat, 30 Apr 2022 00:50:22 GMT  
		Size: 1.2 MB (1180884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695af473b1cd9e144d20d270ac7db7c1e34126fdb27db717ef1b82d4ea459397`  
		Last Modified: Sat, 30 Apr 2022 02:23:44 GMT  
		Size: 5.5 MB (5546712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbdd5d86aa1bccfbc93111261e6b9ae8bbd5777bcb704b395d81b82a8e6f7`  
		Last Modified: Sat, 30 Apr 2022 02:26:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a755bf529bfea3fdd27ac8aa0a2c242d828fd03aa912766c514f925b0d324`  
		Last Modified: Sat, 30 Apr 2022 02:26:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dab9ed6bab5f87837f781c6b6f2631af5cec9d24316a3d8af71d7971b5cf951`  
		Last Modified: Sat, 30 Apr 2022 02:28:04 GMT  
		Size: 103.7 MB (103664283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8f626b8252407df6df973634a2e4356aa55d4b99b403854f663776c11ff2c`  
		Last Modified: Sat, 30 Apr 2022 02:27:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3ed6a9e83e2aa8bc98fc3a7fd76344b5bbe2185f77d65a86c46a9e8ce47e57e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133716329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8861d548374a54940b31d30055fa3ce4692be4ea9418ac6afd0e5bb342237f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:20:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:20:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:25:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 00:25:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:25:53 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:25:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:29:05 GMT
ENV ROS_DISTRO=galactic
# Sat, 30 Apr 2022 00:29:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:29:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 00:29:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:29:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2837428b54ca227343b28e2aebf5f943eb61317acb706203bbd53ccd36b1faa`  
		Last Modified: Sat, 30 Apr 2022 00:38:20 GMT  
		Size: 1.2 MB (1182149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782caaf301f52c6f48c207e662cbaff846f5e221ff2d301aa5123d59be9f9cdc`  
		Last Modified: Sat, 30 Apr 2022 00:38:18 GMT  
		Size: 5.3 MB (5321931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e518f0b96ea742e65f2524920ef0978594bec0e17d20b42b1068bfc73720bd`  
		Last Modified: Sat, 30 Apr 2022 00:41:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be28b19174686f17ae1317ae4d3c9000a0c5da2daba3797916241b4eff9b024e`  
		Last Modified: Sat, 30 Apr 2022 00:41:03 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc429bf8652d7c199bc2696f50eb5d6d96995a020de7042fcefc0c861e53b494`  
		Last Modified: Sat, 30 Apr 2022 00:42:49 GMT  
		Size: 100.0 MB (100040496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24d376e5e7a9471996a0ba2517b9f4860601c4b261f5b4568a13a3138e91451`  
		Last Modified: Sat, 30 Apr 2022 00:42:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
