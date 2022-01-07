## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:0cb0dbe06581dfa142211537c433f649a7da685201eff422f6eb676075d591a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6a85697f6734ef66326a90a302018646cd3b4234990ace51c90eb96ce771cf80
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742701233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b49ae8b9b35c6c2430e8c0b4b0919f03038767d8117d919e894874056b34a1d`
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
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5660e1c9fe436bfbd34680ad650c072c8451ec4dbc87fbd2c5870fa18627eb`  
		Last Modified: Fri, 07 Jan 2022 04:34:36 GMT  
		Size: 305.3 MB (305325841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c6fc7be1b7becb57f8068b6c375101756c09df1fc3cb92b4b30baf97aee61b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645914351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401c6bc42ba54a393d9d03d795b45b5f11695f17f359bf243099c1b9778be290`
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
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb6f19beb6ea8383c29b3d6c750ac3668263f33079b5f9e52e3f9efed7e49dd`  
		Last Modified: Fri, 07 Jan 2022 04:12:45 GMT  
		Size: 260.0 MB (260034872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c4c159951ecb344d4d938be74fdffa8b98eb9f3212b1bf3f32abc667bc3eb2c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.9 MB (702918472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6167b16b39d712390c6d76b4d9e74079934df43eca8cc36cb777c384ddb891a4`
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
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1869584807e21cfd1b68597c82773705ae10af91d3e093729080b38f5138d4e2`  
		Last Modified: Fri, 07 Jan 2022 03:35:15 GMT  
		Size: 291.4 MB (291382834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
