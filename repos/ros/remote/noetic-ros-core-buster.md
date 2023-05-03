## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:06cf4c09a8ee2373792157f32ec540ea08f39a989720f0eedf3c0c50dad1dae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:2863415dfb26f22f0b6318820ccbb6dc7118363e8358a2459d7f6b0862a4805e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300587217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9924f12806821bd9bc09843e0f9f4c5315966616b0631dcd6617687e24f564b7`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1e368f04c44fb0167ff47d43b10fd721c254e2e52f39cf02a2f8e1c9d20bc3ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244600123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0841f2fb87cc10cf6793954ab95d56fde855f4a16509c5a9e94ae9ed297fc522`
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
