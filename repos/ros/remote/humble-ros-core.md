## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:d43aaaae847685889a49a4d9c6b95bba609dafa1071e655f50e499f3bac29940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9563bfd3172e8574e1715fcb30492c30b83fb2df3cf85d3ea29cc7057654b280
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141622125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff91d7a0709c149df8e6061c129ad8b19cad65d1d90d21a7c4dd39918822a3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed4c506a70a1fc02f42a9a6bbceb12d7353f1ee5f1af0f84fcb5e438de32a1b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137080776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffd6f978c34b81f405c704c5a77b8d042c18d88a04910e6d93f2e48a9da3277`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
