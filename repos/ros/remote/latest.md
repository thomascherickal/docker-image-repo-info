## `ros:latest`

```console
$ docker pull ros@sha256:27c748a7718099eb992e11b3930b8f2ab4544c6d1cc64b99fd6b6e1abe820943
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:b84dc55dec6da1ab52de0b8b11377caa867e9c7d37be12ae66752c2e203f8f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232376681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5459f09fa2f11b0c8d454c2b00df1a21b52549f1af3276dfe4230bb864e03caf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:12:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Jun 2021 02:12:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 02:12:51 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Jun 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:13:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Jun 2021 02:13:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:13:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:14:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:14:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Jun 2021 02:14:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7391322adec07e74f2aba8edc862a4e4763771b8e7834acce634c5dbecb658`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae6eda429a76621671058b7c9dedc8b5681069907a1940daeb55913e06cd4cf`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd55023b35263431e19b7c37373a8e1979c28203642348f4a0d7256e5f0d8c56`  
		Last Modified: Fri, 18 Jun 2021 02:30:47 GMT  
		Size: 120.0 MB (119968384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317a9d8f5efbc4f8d5ce6e64424fcea35d4bdd9b37743c6954f5ca8f7a6d96e`  
		Last Modified: Fri, 18 Jun 2021 02:30:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34a9d58406d26b6a333949e85d7eb8c2125734cd88acff81e85bdc7a9b786a`  
		Last Modified: Fri, 18 Jun 2021 02:31:10 GMT  
		Size: 66.6 MB (66602470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9c96e5466b7e460ffeda8aeb7a058303c3729c935f37605673bb581e52058`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 235.2 KB (235216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d51214db13967fa836048e129c5ef2406309f57adff4e76911d9b6ed9a50cf2`  
		Last Modified: Fri, 18 Jun 2021 02:30:58 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c611edea0d9932f52f6a20f67b9c9af4986bd10620975328e7c6bee8160f4c`  
		Last Modified: Fri, 18 Jun 2021 02:31:01 GMT  
		Size: 10.3 MB (10283078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e67ac993be54f63b4f0a99b7a220d970d4fe8d00b304ccefd9bf1be36a66e41c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212756674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1225d3458fd9765460e5d38bdeceaa63debf7aca992d789d08bad856908f3e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
