## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:640c26eadbd4d4b6eae01e694da96212be271e30d8739ad2cb656465d5880c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:4fb4d2c745892e1926e3eadbfdad9c9c39a828a99d6e643414ddeb4310d3fd1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300586898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35052ea48f606b78b488fd973a0b9fdfb349c2ef6a2a4e8260da2fa527731414`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6733f50bf49e5ebc9e9b2f05c47cc1519731c45ea16caab58e3aa86b4ab33462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244569690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d60ce06228047cd37fd09ec239c06f2453b0b8a8646191bc9812abaf869293f`
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
