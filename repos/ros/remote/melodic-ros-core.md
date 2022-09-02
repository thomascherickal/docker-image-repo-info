## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:4d62d17a0c771eb97ef20669aeae1c2b363ca29b7f6d6bd79267a187f1dde4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9b669165378423e81a191798b5e52aa75e944399105596a518f4b552cd63afbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291976206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:379814066976db125a7e5d64cfcda1c2e9f57f003358ac3442eb1e117bae9d7a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:517a5cd34d4f76ea5bd0e123281d4ebaf06483d151b29d5852bcf1199d1462e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266249851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3807b97ce7468b1b2aedbfc07777530bf31cb68749123cd0ee0cf10c2c4f1ae6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2edb6d2cfc7df7d81378db7ca5d7c02275aaab95ed9fa0157e17bb5478bcb154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281338156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2206435ec70b97df1443b70f21da2ec487a4fbce004b232c1c1a9433acad2e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
