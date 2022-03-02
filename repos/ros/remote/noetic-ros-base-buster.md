## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:d8d0895f1c50ba21d84bce7e701147c22ca577f176ccb7ae0ae5c0364b90106d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:f74ba82e15175cee129d5bc5d1566d954c2ccefd2a2f3f3c3dadb8ae506590a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463273887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:453b48768682d6f37b5d6c1086b7e92ad5582750be12d2ed159fe2c8fd0a9c34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:41 GMT
ADD file:e8b516b464e535b435a6ed8609bac98acc90ee30e2a0667f68932f0d924f6e49 in / 
# Tue, 01 Mar 2022 02:13:42 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 10:37:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 10:37:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Mar 2022 10:37:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Mar 2022 10:37:54 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 10:37:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Mar 2022 10:37:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Mar 2022 10:38:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 10:38:59 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Mar 2022 10:38:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Mar 2022 10:38:59 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 10:39:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 10:39:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Mar 2022 10:39:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c9a8b42b5780ac49c71f392c9512c0167ecc23de9b30b1b5f38747b73097d1a`  
		Last Modified: Tue, 01 Mar 2022 02:19:43 GMT  
		Size: 50.4 MB (50437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c133b370766b6f5552e000ccf033e32442276773c2cd08a21a0ac9f18259d3`  
		Last Modified: Wed, 02 Mar 2022 10:43:37 GMT  
		Size: 10.9 MB (10892098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ae26f65841562882d5b66361657c9e58e057d74f3ecdca875adcf248f594eb`  
		Last Modified: Wed, 02 Mar 2022 10:43:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32c03d38883523f98928ace45a667c9a6f9c1e357c09c22bc32e9f75e3ee391`  
		Last Modified: Wed, 02 Mar 2022 10:43:36 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3c4ec48c4a1bce55afcd9bbda77e99d790164b04caa20748eb0bd7b2dd5ae`  
		Last Modified: Wed, 02 Mar 2022 10:44:10 GMT  
		Size: 239.1 MB (239095099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970c2b44800a0ec91c9c10e46c3e219d142dbbce8abf085f6c89e01de485a28a`  
		Last Modified: Wed, 02 Mar 2022 10:43:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f52ffdc8600971c23fcc3470929f8e69fcf2f8140208f05977079961d4c9237`  
		Last Modified: Wed, 02 Mar 2022 10:44:29 GMT  
		Size: 86.6 MB (86566685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b44425534870ef9a16bf44a1fe3fa688b25244bebc0c9fe2c9db6e3107d70aa`  
		Last Modified: Wed, 02 Mar 2022 10:44:17 GMT  
		Size: 303.9 KB (303871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c3bc0c0b6b4ceaa48e62a3d09745513fcedb49c063d68038f3b84cd2ef6909`  
		Last Modified: Wed, 02 Mar 2022 10:44:27 GMT  
		Size: 76.0 MB (75976673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a6f9e01d94995d5ebdc90a7aa8a404c598ab2cea80c225426a61af23251a41ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.7 MB (402736337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f468d0d131a18dfa9ea4ea06d230eac24e5bec1f8c34a89ed2f78a58427b6d59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:41 GMT
ADD file:ec3d90624857dbfae217c1372a38966f453fcd51282379652f07d2ccf6fcc67e in / 
# Tue, 01 Mar 2022 02:11:42 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 22:06:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 22:06:27 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 01 Mar 2022 22:07:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 01 Mar 2022 22:07:13 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 22:07:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 Mar 2022 22:07:15 GMT
ENV ROS_DISTRO=noetic
# Tue, 01 Mar 2022 22:08:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 22:08:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 01 Mar 2022 22:08:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 Mar 2022 22:08:34 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 22:09:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 22:09:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 01 Mar 2022 22:10:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:72f0eb753e825356fa0fef854ac259cc8eefdb0f689516f29b13da8b1595c342`  
		Last Modified: Tue, 01 Mar 2022 02:18:46 GMT  
		Size: 49.2 MB (49223022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81dad0cc65e28099216f8e66fc4a9ff1d7beb908c009b51ce776f53e30ed16e`  
		Last Modified: Tue, 01 Mar 2022 22:15:59 GMT  
		Size: 10.7 MB (10688196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbbf1f406c973f913df3bf3c1a30b098a376a89b1bdb355fa67a4d85c53437`  
		Last Modified: Tue, 01 Mar 2022 22:15:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cb5a189c80ce8736e0a2023d103c32a058bb7dc0ffd1788e9621c793e613af`  
		Last Modified: Tue, 01 Mar 2022 22:15:58 GMT  
		Size: 2.0 KB (1952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f4e8ce419e89e72b01e8ac6833ae7d79adf8b984203a468dacae04d36dbc01`  
		Last Modified: Tue, 01 Mar 2022 22:16:29 GMT  
		Size: 184.3 MB (184303647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47f84d9b6f883f86b5ab85b7341f781dd8a4f20c3576334ec2b1b2511b39120`  
		Last Modified: Tue, 01 Mar 2022 22:15:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823c701829b09ea926c81cf7d31b4ce9fa4d4990e4d494dcc244816cfbb6f59b`  
		Last Modified: Tue, 01 Mar 2022 22:16:48 GMT  
		Size: 84.4 MB (84351038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d8e0cf44deb036ea2133c6e3b736cea94b5676c0043de056918a76f8693cbf`  
		Last Modified: Tue, 01 Mar 2022 22:16:37 GMT  
		Size: 303.8 KB (303820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b401603f0a64181e3faea2a2fedbe6b9d6528a442bc2163aef25c8efaba1757`  
		Last Modified: Tue, 01 Mar 2022 22:16:48 GMT  
		Size: 73.9 MB (73864242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
