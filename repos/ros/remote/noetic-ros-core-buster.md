## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:2e800aef442eb1c7ac4d0dc992077320abfd89980d7cc5f6ace265d178cf5c76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:01366ef13d56050834f595349bc90ab8ae4359b56eedba140cfcb80ef2a36263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300381406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303e70ddcefe851421ed225be4fec71d1d962061c0b5bb14d1228dd5544eca97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:54:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:54:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 14:54:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 14:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:55:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 14:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 14:55:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a25b8c075beb4891f7c9088956d2a452f32036d8126e37217b5b62fd7024c`  
		Last Modified: Tue, 17 Aug 2021 15:02:09 GMT  
		Size: 10.9 MB (10891952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b43ac20734a706cb03369661415e15f6856a48275dcd4fe7744b0bde5d23`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b19825ce46253a4664a6e606382250ba22ec8d0e1d13516be7d225efcca57f`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034eef40d3fabaea23b5d4473263a3a6ab8cd3545504c1ba16818b3b90152d1f`  
		Last Modified: Tue, 17 Aug 2021 15:02:50 GMT  
		Size: 239.1 MB (239050839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae7d371ba1fee4f46bf91b9a18289de1dd3472eb2c3b8458f8ff2df5825c78`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0684d6a87e895094574883528a51ad31c58a2453bfef73981f32b487db50d859
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244347695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42db978a3ff3a7a18a119b3b59d7ad9a553dd993a7e9d9a36d856549935cc4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:27:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:27:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 03 Sep 2021 11:27:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 03 Sep 2021 11:27:50 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:27:50 GMT
ENV LC_ALL=C.UTF-8
# Fri, 03 Sep 2021 11:27:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 03 Sep 2021 11:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:28:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 03 Sep 2021 11:28:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 03 Sep 2021 11:28:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1462dbe8ebf1cb3c2f5806cb19d8c66f38c095230d7abce37bddb2ba968ca5bd`  
		Last Modified: Fri, 03 Sep 2021 11:35:40 GMT  
		Size: 10.9 MB (10883319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2664a95765076375c283614578526207643956bf3842410bcc7bf4d68dee1862`  
		Last Modified: Fri, 03 Sep 2021 11:35:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b32b930665db018324ae169bf319ec4667a22080016cfe417f1c301a301bb`  
		Last Modified: Fri, 03 Sep 2021 11:35:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b848e0f07ce6baab097af02bd4e576eb86c8e1b06351507016049cb42b6631d`  
		Last Modified: Fri, 03 Sep 2021 11:36:12 GMT  
		Size: 184.2 MB (184239824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0fa9131028a94f4fffe644b96939f628590f4295592695f28746a9e10984b`  
		Last Modified: Fri, 03 Sep 2021 11:35:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
