## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:a16987d5d6729ea57d120332059ed56e1eb7612a7f9aaccafa83a55c00c4c790
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:2d40d32907926aaefb11b4c7dcbaeebf52103d598cbd394c12ec86b40c97e692
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.3 MB (951320221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46af7519e58644cbc3d57322cc816d396b8bda1ddf41c1b712fb5e975537ab4a`
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
# Wed, 12 Apr 2023 09:49:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4260926addb6a4d57ccf566574df11b0c4c215a725f15d5b8fb228241f92f3f2`  
		Last Modified: Wed, 12 Apr 2023 09:52:23 GMT  
		Size: 487.8 MB (487817262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:980152242b671d03db9a26efee4daf2633661b4247037bbd3acc946f3ac4444b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.1 MB (868115447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e8b5202e5fb2faaf4a1dee3bd47c886e64dc7f1589ca5a6b67bb2579e11c30`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:17:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:17:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 03:17:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 03:19:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 03:19:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 03:19:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926daaa3f39d210833d9a3a75b2e33aafd38f4adcda623bb40686f5480d8eda7`  
		Last Modified: Wed, 12 Apr 2023 03:25:46 GMT  
		Size: 10.9 MB (10902667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ef889428a3c0c2686a4bb8d4e5af08778a1b25251d4873a4635b0b2af721d8`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b211d556fba373cffc4c30d24942793ca6d51c78179037897e5f465fc65e4408`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161bac3145a70b13a85c49796d22151dc27a76ea04b256183b318cc9efc8686d`  
		Last Modified: Wed, 12 Apr 2023 03:26:06 GMT  
		Size: 184.4 MB (184427087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91b09fc5f446950a1e8e392c05737de9820b95e50745e93232b6ff4dba0617`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d31bfc2a7fad06ba1563ddcf7f96daf937621936041ba76fb2e42b45d9f327`  
		Last Modified: Wed, 12 Apr 2023 03:26:21 GMT  
		Size: 84.4 MB (84395801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ec420fccc4bc3cf3805910ff22f8789cd48387fcefed5829785ab9279e8e9f`  
		Last Modified: Wed, 12 Apr 2023 03:26:13 GMT  
		Size: 313.0 KB (312977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e8033e5e52d2e2310af7d82b5846e3f1900897dee49ceb23bf0721dac3353e`  
		Last Modified: Wed, 12 Apr 2023 03:26:20 GMT  
		Size: 74.1 MB (74090563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c366ae282bf50e572d970fd7d54011aaa06faca583dc1548110f0865cdc3809`  
		Last Modified: Wed, 12 Apr 2023 03:27:22 GMT  
		Size: 464.7 MB (464745308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
