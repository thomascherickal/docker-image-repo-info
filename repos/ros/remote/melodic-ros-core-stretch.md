## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:6d73ffc37a163f08ab19b1193821e1a22fd3b2b5691a2b8c99b0d2aef63aec9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:1d50fd705f74bfa15cafc1463c1cab0a12cd9b34929ab203794a2a71389566d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.2 MB (322160460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84add7dd9acdf9a46acec10c6798fcaa7dbec933acdf897ee55ba21c62d8e6cb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 19:22:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:22:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 10 Sep 2020 19:22:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 10 Sep 2020 19:22:53 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 19:22:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 10 Sep 2020 19:22:53 GMT
ENV ROS_DISTRO=melodic
# Thu, 10 Sep 2020 19:24:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:24:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 10 Sep 2020 19:24:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 10 Sep 2020 19:24:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba185f65d54db323ab946a5e9c37dfade8c963fd7c77e40ebf7103a1404461`  
		Last Modified: Thu, 10 Sep 2020 19:35:48 GMT  
		Size: 6.9 MB (6866928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e93f0c8bead1f4a636ace143d7195fe34ee2830234cb5a4c761b965b089ada`  
		Last Modified: Thu, 10 Sep 2020 19:35:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f07b60a04aae8b7b5012f737d7740e689bd88eea45f68e6eca966b8f046a79`  
		Last Modified: Thu, 10 Sep 2020 19:35:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ecfead1d8fe71517621403f3b5838209a45ae3d6072bbc92c5b20fc9de4073`  
		Last Modified: Thu, 10 Sep 2020 19:36:53 GMT  
		Size: 269.9 MB (269924988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dca37c3796b019ae079bc6432f1760cc1e58c52d84dca9a8bd117813430be8`  
		Last Modified: Thu, 10 Sep 2020 19:35:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1ffc873a24d2de8d07363d13fed784e92797c1ffb81fadf62ea30a4794d976f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.6 MB (274634281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1093ead4aa456d7aef7528f2e101a756194850480f0403bcb69ed43b2c7eae`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:23 GMT
ADD file:f74bb8d38ef70a022988428f254630d1f424ed9a3b957687b0cd0f85b9d49e29 in / 
# Wed, 09 Sep 2020 23:54:25 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:49:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:50:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 10 Sep 2020 17:50:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 10 Sep 2020 17:50:21 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 17:50:26 GMT
ENV LC_ALL=C.UTF-8
# Thu, 10 Sep 2020 17:50:29 GMT
ENV ROS_DISTRO=melodic
# Thu, 10 Sep 2020 17:54:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:55:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 10 Sep 2020 17:55:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 10 Sep 2020 17:55:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3b396f138ad78ffceac749b105c676dce568fa15a7b9f2273c2ee13ba023cea1`  
		Last Modified: Thu, 10 Sep 2020 00:01:33 GMT  
		Size: 43.2 MB (43171697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfa29a8456bb2ebaef0eca491538c026723b1f78edb1a107569756d2a3ce15`  
		Last Modified: Thu, 10 Sep 2020 18:26:17 GMT  
		Size: 6.4 MB (6440792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82b5af61f8168bdb9f6ab1b7c9f527bf108fa930fe26b10e944e45d24a0ca5`  
		Last Modified: Thu, 10 Sep 2020 18:26:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8570d91b0afd4af1ff2447141b92ed7ed471251fd9dbea0da2488b14076d7ceb`  
		Last Modified: Thu, 10 Sep 2020 18:26:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ea2bf9d7559afeca0cb6b14223851a53a5095de6b0276a34e4c771a53eba2c`  
		Last Modified: Thu, 10 Sep 2020 18:29:47 GMT  
		Size: 225.0 MB (225019969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a962f8b50b62e542f16e34961b364c107269e8cce651cf1d923e3ac9ad28d`  
		Last Modified: Thu, 10 Sep 2020 18:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
