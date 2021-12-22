## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:9f7204ab243d5df4c9f1b2a4b088bea6b8cfffe86fda3516cafca8b897ad8246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:0e72063b55d6fd36382fe96279a3521dab05eba87af044036a4579cb3833d923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300420756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843649105be24214e63135218c4d1bb8d004608854be280bc2defe7bdffc3bff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:56:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 23:56:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 23:57:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:57:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 23:57:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 23:57:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a21eb75d0e3012979c6611472ad2ce77f9603178d355b33e3a29b873c09cd17`  
		Last Modified: Wed, 22 Dec 2021 00:03:48 GMT  
		Size: 10.9 MB (10891938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a0355b4bb6623abb06a5060650fda200f613e82ff0c1660f1dd412468468d`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428381b1469052a8549b56c928ac7628c4b0b3212ab6a0e15cd9a7cb0836f7cb`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb2dc8dfc87f5650375873e92661d1220cf0d1ef485c60f8350795669a60fb`  
		Last Modified: Wed, 22 Dec 2021 00:04:21 GMT  
		Size: 239.1 MB (239089267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5280b24f54ae8eeabff880a2eab6ce4c01ea397fe51e158a984ddcc9b1812a`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:20d0f2c349578d271200aea73e741c8b718409786a372a03b04be558631f9d9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244216048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf549d683df4e6b860fdeccfae209621f923f4a014cfc94191db0657fc7f8be0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 09:38:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:38:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 09:38:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 09:38:25 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 09:38:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 09:38:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 09:39:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:39:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 09:39:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 09:39:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedd2aa81cc2e7379bd59690f90cbd16cf4e588be2a502ac12108e4ba75a9cdb`  
		Last Modified: Tue, 21 Dec 2021 09:47:20 GMT  
		Size: 10.7 MB (10687984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00429e5154d2608cfad408e0de2499d94136b3ed658f2dc5aad48fc80c44537f`  
		Last Modified: Tue, 21 Dec 2021 09:47:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d257c405577ebdaffc9dd7205a3033020e775049c0cc3c0101939fa4bb51bbe`  
		Last Modified: Tue, 21 Dec 2021 09:47:19 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4366b7170e598cb5e67f80d349915ed2decdb84edf3cee3f5777cc668a8ae`  
		Last Modified: Tue, 21 Dec 2021 09:47:50 GMT  
		Size: 184.3 MB (184302551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5b3f41b835902abd4dc52846cd889491aca26b96b40a266e9bcb92a168c20a`  
		Last Modified: Tue, 21 Dec 2021 09:47:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
