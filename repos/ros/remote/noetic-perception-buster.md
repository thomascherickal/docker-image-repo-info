## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:66687b4c572cd307bf01f7e5c298a572b27e42c3296402615b378052c1295f1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:7f82161c2bf10db0c197628cec8ecec0176478f0c639f0c63c26b3c24ba79f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **967.6 MB (967645106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:414d48468c4d758a2434d893cd2338661b856fc454e4cc0beff0bbb7b573f613`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:08:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:08:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jan 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jan 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jan 2021 01:08:48 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Jan 2021 01:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:10:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Jan 2021 01:10:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jan 2021 01:10:27 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:11:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:11:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Jan 2021 01:11:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:16:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472a295ebd41d3968f8d863e1015d367c18e985c1c0f56d543463857ec9647e`  
		Last Modified: Tue, 12 Jan 2021 01:24:06 GMT  
		Size: 10.9 MB (10890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d374fcbac4a1edeece11e802c028e58bcfd68f594a873fe3daa75cb39560a5a`  
		Last Modified: Tue, 12 Jan 2021 01:24:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e0241a79b24e9ee7ee6f9df3d32a58e6a527c754d734ffdeab34eb9f7d189`  
		Last Modified: Tue, 12 Jan 2021 01:24:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090f94ca05cb3b6e59c6c7edda6c987adc2e22ba0327be09a7d9209b23653182`  
		Last Modified: Tue, 12 Jan 2021 01:25:15 GMT  
		Size: 238.9 MB (238919824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a4f8987d94cbf12fbebd2ede2b2e65b75267777ba507219d725e88a9a5cb21`  
		Last Modified: Tue, 12 Jan 2021 01:24:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b600712acb247824ee23a4eb56fa59e128ee396bf36b595f1e74c7421fe03eb`  
		Last Modified: Tue, 12 Jan 2021 01:25:53 GMT  
		Size: 86.6 MB (86563501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e7c2dfc7eb08cc8406fb38c8de6b7a3415b24b609e877ee9a2a590b64df5ce`  
		Last Modified: Tue, 12 Jan 2021 01:25:23 GMT  
		Size: 261.2 KB (261205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf02b5e910f2c0aabe6b7afcfee54c2b7c8d48e2d345983eab101a31b3b6a7d`  
		Last Modified: Tue, 12 Jan 2021 01:25:48 GMT  
		Size: 76.0 MB (75966525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9cd1b9a1ab2f727cfda3f84f0d8c78ac64d4a99f3cd9b639b5fdec06f1a8e1`  
		Last Modified: Tue, 12 Jan 2021 01:28:32 GMT  
		Size: 504.6 MB (504642732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3d249001e2ae36cd1da431e9579a3391e4b9800e7958e6c4ae652729da70436
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.5 MB (884479084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f36e98c97fb44facea5f545a2107279efea5802b9c678e78e4cad8019d9a7059`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 23:25:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:25:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 11 Dec 2020 23:25:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 11 Dec 2020 23:25:11 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 23:25:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 11 Dec 2020 23:25:14 GMT
ENV ROS_DISTRO=noetic
# Fri, 11 Dec 2020 23:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:27:34 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 11 Dec 2020 23:27:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 11 Dec 2020 23:27:36 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 23:28:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:28:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 11 Dec 2020 23:29:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:34:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6802a596e847ecc40fc64a4020bce9c6b7ec241a9a0adff6a2f4b93c30b2144`  
		Last Modified: Fri, 11 Dec 2020 23:41:10 GMT  
		Size: 10.9 MB (10882958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d048a0e9c93d12fc2502ef2bd5aff74d265481bfe6a09ed85acc1b9d28d689`  
		Last Modified: Fri, 11 Dec 2020 23:41:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89503d24c7d28733c7447800ad677d2131c8d16d0a168ebb554b2b3daaf1a1f1`  
		Last Modified: Fri, 11 Dec 2020 23:41:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215ec51670c89e647b8382b61d566bad5238b2661b6575cae78036b6dbc1da44`  
		Last Modified: Fri, 11 Dec 2020 23:42:01 GMT  
		Size: 184.1 MB (184145865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f19aa0624291920427cd6503ba38ebd048f0d00f4e6f303a9893c73a1d212a`  
		Last Modified: Fri, 11 Dec 2020 23:41:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1e404c27ce42d1a86ea2b5f569c72e14662afd6311cc8246e7404d572a91b3`  
		Last Modified: Fri, 11 Dec 2020 23:42:31 GMT  
		Size: 84.4 MB (84354929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fcf8820144a3531ad73680a7bcfce89b628b8f63a4633f46f390320c0a5778`  
		Last Modified: Fri, 11 Dec 2020 23:42:10 GMT  
		Size: 254.6 KB (254605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e4418084bd7fe7d75ffae62f54e83367b6952bf4674aa4cd51cc4d27d10b96`  
		Last Modified: Fri, 11 Dec 2020 23:42:29 GMT  
		Size: 74.1 MB (74088219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9512398ecd63c39953f3eadb4e1b6ac63f76aaa997eb5dfda4d511f2102afd`  
		Last Modified: Fri, 11 Dec 2020 23:44:48 GMT  
		Size: 481.6 MB (481570352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
