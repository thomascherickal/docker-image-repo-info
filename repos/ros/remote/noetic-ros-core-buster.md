## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:e23b0f094d3b73fa72eb3f180e9ca7071ebc650eb0a57b156559cc63cdb5b221
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:a1c6c0044c06dc2184696ce9aeae3507f2120f94223ef6a1196f684c786b0a6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300524291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c6fee82ad06853879bbd3091f717f1719d29f43ec3c213f006f9e8459bd547`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:25:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:25:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jul 2022 13:25:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jul 2022 13:25:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 13:25:16 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jul 2022 13:25:16 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Jul 2022 13:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:26:18 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 12 Jul 2022 13:26:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jul 2022 13:26:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52944b008d648ec10b90034e858c8a366ad6963623d2cd548e94f3b211c510`  
		Last Modified: Tue, 12 Jul 2022 13:31:01 GMT  
		Size: 10.9 MB (10893460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f428e8ee180b2ced991a099c7188b1e31317b70123d54f213c181337fbd54bc5`  
		Last Modified: Tue, 12 Jul 2022 13:31:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab13f730c1507e856b3b26e49c4be43c743c93a6aaa77f01788e3835f0a8009`  
		Last Modified: Tue, 12 Jul 2022 13:31:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5734a0ec049bcdaee22ed9dbea626ae1d18eb539faa26bd4910bbb4b0fe63c2d`  
		Last Modified: Tue, 12 Jul 2022 13:31:34 GMT  
		Size: 239.2 MB (239187862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cd1662d758fe3cb4dd7834fb07702059043ee92feb54312164af4bc4b718e`  
		Last Modified: Tue, 12 Jul 2022 13:31:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:84f96828f39aee595f8614d70466b274a0ed49dab231f8804b068ede598aa4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244293545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:debf14ac309c743939181156899aa2cfbec1a71008241693dca29b060dd1a6ad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:00:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:00:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jul 2022 13:00:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jul 2022 13:00:51 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 13:00:52 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jul 2022 13:00:53 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Jul 2022 13:02:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:02:13 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 12 Jul 2022 13:02:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jul 2022 13:02:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9d4034dfbab9d3d5107231bf79f7e9128aa4489cba93d97578d760166fe3e6`  
		Last Modified: Tue, 12 Jul 2022 13:09:17 GMT  
		Size: 10.7 MB (10689263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0120a667e47e68ebbd4a03de6b0932ea25a0078d49f8ee71a75c9ebc31fbeef`  
		Last Modified: Tue, 12 Jul 2022 13:09:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0820f1a42597e95311859510855953092a4ac35c4d590417693b084968c31`  
		Last Modified: Tue, 12 Jul 2022 13:09:16 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66081e680fda062b62d547ed9e29d0766f71a29d7a5fafb291a118efb1d184b`  
		Last Modified: Tue, 12 Jul 2022 13:09:46 GMT  
		Size: 184.4 MB (184372986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b195084a0c638927568ddb99e45b6b5b0c4d9994a11d7938842a8d3a60a9a1c`  
		Last Modified: Tue, 12 Jul 2022 13:09:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
