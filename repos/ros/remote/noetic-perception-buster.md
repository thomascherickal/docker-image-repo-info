## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:966a5eecf2f9e2b6508f18e8e993e43cfd5bdb2ce485667cd2bcda9f908b1704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:757813b4e28c2434adab9df264ea30b524608fa87f72acf68beb26ea9b541b02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.3 MB (951346769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a390071e96f433888f357032ab666982178c4fd66c01826b84356a17e0f08b18`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:38 GMT
ADD file:f5e6e6cbfbb36f50f49f06fbac953a130383acb67a1c5e9979441f1915b1077d in / 
# Thu, 23 Mar 2023 01:30:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:55:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:55:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Mar 2023 14:55:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Mar 2023 14:55:57 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 14:55:57 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Mar 2023 14:55:57 GMT
ENV ROS_DISTRO=noetic
# Thu, 23 Mar 2023 14:57:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:57:27 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 23 Mar 2023 14:57:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Mar 2023 14:57:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:58:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:58:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Mar 2023 14:58:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 15:02:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e2befb7f5d18aa27b3619ddf1b93607e62ca82d0c627557537c149893346d86`  
		Last Modified: Thu, 23 Mar 2023 01:34:40 GMT  
		Size: 50.4 MB (50448639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6e6f6091b92ed07213d644f33e47d06757c8ca846e3d9a92c276d9c5fc330`  
		Last Modified: Thu, 23 Mar 2023 15:03:40 GMT  
		Size: 10.9 MB (10897008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbe51e5bdfc4bbbd1863dc733210842df4d4773451ad3e3b97158a12c75d3f`  
		Last Modified: Thu, 23 Mar 2023 15:03:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da2fadde18416a222a60396cc301bfff00c8711e0e97d1310a94069eccb2b3`  
		Last Modified: Thu, 23 Mar 2023 15:03:38 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dd060cdb612260d95ac8b282e306e49400054b218aa4fb72f4aaa4f9f73a15`  
		Last Modified: Thu, 23 Mar 2023 15:04:09 GMT  
		Size: 239.2 MB (239238838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03121257a2ad34392087234c38a5c370cf1e3bf6b3d297da74d7d92db294fe5b`  
		Last Modified: Thu, 23 Mar 2023 15:03:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47f986fd943fc96c63708211cd0029fd4f4a1ce0dae877067bcfd2542a709e3`  
		Last Modified: Thu, 23 Mar 2023 15:04:27 GMT  
		Size: 86.6 MB (86624647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567e0013c342030410d9c35f66aaa240bf6a9f0fd8e2861bba61f268f832408c`  
		Last Modified: Thu, 23 Mar 2023 15:04:16 GMT  
		Size: 311.9 KB (311926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f32a3234d59d9cfb3f15c364a962ee5ed705cc1f608a38154c5fbdb5186b5e`  
		Last Modified: Thu, 23 Mar 2023 15:04:25 GMT  
		Size: 76.0 MB (75978138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ca0a8d59c74383fd3d3a52a7fda61bc16f896edfa9e4ab93d2d0d83a560c6b`  
		Last Modified: Thu, 23 Mar 2023 15:05:51 GMT  
		Size: 487.8 MB (487845160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f31847fe252f98c712f11a5e23d975dac4c6672cb0c7842bcb69042bbae3469
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.1 MB (868139167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f235c0a862f7f73f6128321a50568ff37be65f27c572df607589c338f955e02`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:16 GMT
ADD file:35dd833b036748f887e8224e9c5f09846aa5d1d6e1798d12a6355c28e0a087d3 in / 
# Thu, 23 Mar 2023 00:45:16 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:33:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:33:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Mar 2023 13:33:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Mar 2023 13:33:59 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 13:33:59 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Mar 2023 13:33:59 GMT
ENV ROS_DISTRO=noetic
# Thu, 23 Mar 2023 13:35:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:35:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 23 Mar 2023 13:35:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Mar 2023 13:35:29 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:36:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:36:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Mar 2023 13:36:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:40:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a9fffb8d1cb480140dc56a24c58a5d1a284109cd8a640a3719bcda5963d1298`  
		Last Modified: Thu, 23 Mar 2023 00:48:25 GMT  
		Size: 49.2 MB (49239721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b91b6ee30b4f087c1ea96a05e201aa3276826cf050c362f762e574ea8d86196`  
		Last Modified: Thu, 23 Mar 2023 13:41:47 GMT  
		Size: 10.9 MB (10902622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d333b25ec98b602feadfb03e74536f86cb100c88c3ae41708f4f69207cbe5ea`  
		Last Modified: Thu, 23 Mar 2023 13:41:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898783a42a69a03c055068412e53662687477c3f7dd14e4799ce9b2e7ad2e20c`  
		Last Modified: Thu, 23 Mar 2023 13:41:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315cb2c48234779972c6290c195d46ff35df3ccfa9bd8fd99f77ea76c46012e1`  
		Last Modified: Thu, 23 Mar 2023 13:42:07 GMT  
		Size: 184.4 MB (184424937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b25a7c52da25a6ef93080a6fe8585d11832b187dce74bd60fed4d5a82e2d8d4`  
		Last Modified: Thu, 23 Mar 2023 13:41:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45effc9bfe53f0f750c14f05cc2f6f747a574f920f4ffc8b468619df3a9396e`  
		Last Modified: Thu, 23 Mar 2023 13:42:22 GMT  
		Size: 84.4 MB (84396211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff11d29eadaaaed8e78ac3a1af2fec7af17763b0d5b042052de27a72812a51e1`  
		Last Modified: Thu, 23 Mar 2023 13:42:14 GMT  
		Size: 311.9 KB (311933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9201db444334b555a4071e530d520b57917eabb315553569cc81642b055e1e`  
		Last Modified: Thu, 23 Mar 2023 13:42:21 GMT  
		Size: 74.1 MB (74090536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c760bb06044cd19ce2f9810d59cfe772b4ab7ebfdfc06eff7369d46e78b0451`  
		Last Modified: Thu, 23 Mar 2023 13:43:23 GMT  
		Size: 464.8 MB (464770797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
