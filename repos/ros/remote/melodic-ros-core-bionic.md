## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:50f269b0b49d03ccd82ccbb218f67d8c2d5c4cfa31653a9244aadbb2f4f7c034
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:bb3438831733d7259a71546d7ab92a3b3ad1ff0c1326aaf1d5abd4536fb52a4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291868889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75506b391d30e869af6d027c5baaba17b6ef62ac7fa7b670dad24d207c337744`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:636f37a5d033d998428a18ab30152404825f8c7f2dde56d586c35987b8c10935
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266152548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5aa91d6c4305b8309cd446a9cbc96c231d2da7ffd19240a281d546e9709a63c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:56d06aefa375942722d64ad261ee56402ec50704cc0e60414a7115b645f57b97
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281190173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92f626f8ecb30009f8a752384bce5a1626cbd813f7f29ccf4e4f3d3d8774d5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
