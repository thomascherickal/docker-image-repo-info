## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:f6333591ef1ba3acac19ff94cafe99632293efcf87c7c903656da513bb1c6cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:8be6a4017ab924705d204b5543bc735d6f2b24ae7aa0218b075df7dc7be56a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484659940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037652e029b16ee89f1f44c33ae00f3c5372c84d731d01eba0a41dd42349f6c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:42:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:42:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 09:42:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 09:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:43:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 09:43:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 09:43:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:44:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:44:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 09:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b00ed65624414cebfd59eb932346275e83df42e1422d20a7b14c8c9edeb48a`  
		Last Modified: Wed, 12 Apr 2023 09:50:13 GMT  
		Size: 10.9 MB (10897019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b3f5b658f43273d64d1a1aeea2487b1b9970a33e08f5a29563764943265a0d`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb716cf3c7952570768bfd3fc5fccb036e9a0beb781e9291a6e11d3f460c93cb`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95e1cb6890794f51bf3e91eae05d0594612953151193fce93420de5a9145f71`  
		Last Modified: Wed, 12 Apr 2023 09:50:42 GMT  
		Size: 239.2 MB (239239058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2534899cbc0a30e85913561bf4af251fd949395ba14ff3352a4afcc7dcf4e8`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0454600fb4adeb722ace480ea8933b040d3b48fdd7d28c7082eced41a81434f5`  
		Last Modified: Wed, 12 Apr 2023 09:51:00 GMT  
		Size: 86.6 MB (86624654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4401a00ee0597bf328d3f44d15501ac656165b052d153dcbd298a69c447af0`  
		Last Modified: Wed, 12 Apr 2023 09:50:48 GMT  
		Size: 313.0 KB (312981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e121b0feeb32a176d80b2d8ee992747b9c8498669bc20d20b92eedf867ec8890`  
		Last Modified: Wed, 12 Apr 2023 09:50:57 GMT  
		Size: 76.0 MB (75978107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e0ecca7cd4d691fe5a4de7b009310f1e21326d187c068f6347d3cebcc4ed35`  
		Last Modified: Wed, 12 Apr 2023 09:51:09 GMT  
		Size: 21.2 MB (21156981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:62b331583d881703aa3722cb01832e369827a54ed42d0f5644eeb624ed7bfadd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424200671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384665c219d79e6d596ff456bd49b0074781ec6579ff636272c9b64aac094356`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:56 GMT
ADD file:6042e29dcf5e22439cd69873d8960f8d3977abe915ef462aaa84368a7186a3bf in / 
# Wed, 03 May 2023 00:22:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:32:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:32:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 18:32:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:32:32 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 18:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:33:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 18:33:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:33:54 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:34:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:34:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:35:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7c5fe8e0ac53c77142bf16686fc01d0d2b1fb2da7be5414cdf2f224ec485592`  
		Last Modified: Wed, 03 May 2023 00:26:10 GMT  
		Size: 49.2 MB (49238630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4b1b3aff79daeba459c24d6625912443a9c4b6e072fd443df8cf1fe609a3b`  
		Last Modified: Wed, 03 May 2023 18:59:14 GMT  
		Size: 10.9 MB (10902746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bd0f1f3ef8032558026a60ca367a9d7b0a28a5d5656befe67922b145ce30bf`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ffa192fc268fe17d966f4b3cea0d44a2889b03c6266a5d26e16c239241f65e`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66412823f7f9778ca86e89b006f993392e02d4dcf6d72bececff2961ab62e97`  
		Last Modified: Wed, 03 May 2023 18:59:49 GMT  
		Size: 184.5 MB (184456335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220fcae6736a0fef7e49e980a9743d78ac71f0793d181838e243ca8df2e17b7`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb95d7c1cbf0d06fe344363abab7d53bcf3e9530c86b6b5d15445e3456dc5f`  
		Last Modified: Wed, 03 May 2023 19:00:03 GMT  
		Size: 84.4 MB (84396518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35bfb55f24afd444091072d43309bdde850dfe001b51461b00b1341cd892783`  
		Last Modified: Wed, 03 May 2023 18:59:55 GMT  
		Size: 292.5 KB (292488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9887f28731774c4b067f23703dec47affd41340f5bf051055b087050dff54a`  
		Last Modified: Wed, 03 May 2023 19:00:04 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b56d67b24627b9c34d7c74e4216c7df0077cb8e6fddbee61d2b611db7cc6652`  
		Last Modified: Wed, 03 May 2023 19:00:16 GMT  
		Size: 20.8 MB (20820893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
