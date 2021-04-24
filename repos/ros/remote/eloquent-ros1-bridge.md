## `ros:eloquent-ros1-bridge`

```console
$ docker pull ros@sha256:b28a4e7abef8624c3574605ccb318ff6ccfa920b1b250f26c3aa27c763919431
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:c7c311b41d3168e70d4f4e6f2cb58cda71f32eaabecc3d2993c5edb5c4cb7347
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **504.2 MB (504227441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fba15cccba4d40364a7d5a855e7b8a9d940bf44ee8135a1b6a4a4ed575eae5e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:54:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:14:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:14:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 01:42:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 24 Apr 2021 01:42:32 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 01:42:32 GMT
ENV LC_ALL=C.UTF-8
# Sat, 24 Apr 2021 01:49:34 GMT
ENV ROS_DISTRO=eloquent
# Sat, 24 Apr 2021 01:50:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:50:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 24 Apr 2021 01:50:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 01:50:30 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 01:50:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:50:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 01:50:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 24 Apr 2021 01:51:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 01:51:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 01:51:13 GMT
ENV ROS1_DISTRO=melodic
# Sat, 24 Apr 2021 01:51:13 GMT
ENV ROS2_DISTRO=eloquent
# Sat, 24 Apr 2021 01:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.10-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.3-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:42 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfad5d88235e65844b7c8944e2bd9a0cacde3a1ea196f87712547e7b0a19c3f`  
		Last Modified: Sat, 24 Apr 2021 00:17:26 GMT  
		Size: 841.6 KB (841642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f3d2f3c3421256e6ecc54a8595810a16a332c15bd766038a835b1277f408ed`  
		Last Modified: Sat, 24 Apr 2021 02:05:22 GMT  
		Size: 4.9 MB (4873267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c9b930401af839e1ced7347be568d3de35f7c40e267d68a500f0eea8b00578`  
		Last Modified: Sat, 24 Apr 2021 02:05:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab3e1d3c2b45ea3515d8586091fb493b93ab53265024e5569f468c6a9b94b2f`  
		Last Modified: Sat, 24 Apr 2021 02:11:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42835e3b41af3ba6bc92d60c3cb729d31e36b1cfcdf68246845ae30d066e5c87`  
		Last Modified: Sat, 24 Apr 2021 02:13:55 GMT  
		Size: 183.0 MB (182989357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b71aad171acab46fb45b5ad2e8cd36eda24f5b9ff1c865f0dee3293b1635d42`  
		Last Modified: Sat, 24 Apr 2021 02:13:22 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1115b8adb620211c2bb2c0bc3eb6c5844bda2e4ab62a08be65592d592d7da32d`  
		Last Modified: Sat, 24 Apr 2021 02:14:21 GMT  
		Size: 63.5 MB (63530758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5c22c9cda3f7d5c9f639af7834b21e51e92c8d5076dece18928ecc3cc78728`  
		Last Modified: Sat, 24 Apr 2021 02:14:12 GMT  
		Size: 205.4 KB (205373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2813a0bbe4be8ebcefcc591cd56aca11d0fc594cb7f0f8bdb9a3031e5e09ea07`  
		Last Modified: Sat, 24 Apr 2021 02:14:11 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b31787eb9932d6aa70bb4c07e0d3c94f67bd3dda6b9da1bc81bb3c10540bd6`  
		Last Modified: Sat, 24 Apr 2021 02:14:13 GMT  
		Size: 4.6 MB (4589101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485c3c3c16639357fc1416e1eac12e819e4310e8c9292dfbee93cae3c8d5da1d`  
		Last Modified: Sat, 24 Apr 2021 02:14:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1b078245f6ae370fe7464fca6a373c84e3402f03141bb7be004e6f7a28dcae`  
		Last Modified: Sat, 24 Apr 2021 02:14:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1831624a9ef773378da594383642d3ac0aa630c2d502103939d9f05fca00c60d`  
		Last Modified: Sat, 24 Apr 2021 02:15:03 GMT  
		Size: 117.8 MB (117769290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e027fadcf3c0412345f62f59752d133f3b9df7da866cc0162eb9c5f25a720c5e`  
		Last Modified: Sat, 24 Apr 2021 02:14:59 GMT  
		Size: 102.0 MB (101987119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7835875a52757a2a369d83c3a2c2be1c28fe9baa232e227207b5296d2efd9f`  
		Last Modified: Sat, 24 Apr 2021 02:14:37 GMT  
		Size: 739.0 KB (738988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cbf6c90a0e7065ab22a5ba8cb489f48e8477c10dd320d3151e908c7f9cacb9`  
		Last Modified: Sat, 24 Apr 2021 02:14:37 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:937226d16d811ef9e6590647b8b4e0ef7171422e80eb060e7a020572a8d3d5d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429053186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d50d792350d607ced269223d028ba89d36e278cecaa110063f626cdbdd5d9bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:36:14 GMT
ADD file:2aae46c08b4df366cc04262aee873d11018c693dd09df0862d54c9ae71cd75b6 in / 
# Fri, 23 Apr 2021 22:36:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:36:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:36:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:36:23 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:32:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:32:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Apr 2021 23:58:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 23 Apr 2021 23:58:23 GMT
ENV LANG=C.UTF-8
# Fri, 23 Apr 2021 23:58:24 GMT
ENV LC_ALL=C.UTF-8
# Sat, 24 Apr 2021 00:09:30 GMT
ENV ROS_DISTRO=eloquent
# Sat, 24 Apr 2021 00:12:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:12:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 24 Apr 2021 00:12:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 00:12:29 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 00:13:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:14:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 00:14:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 24 Apr 2021 00:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:16:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 00:16:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 00:16:20 GMT
ENV ROS1_DISTRO=melodic
# Sat, 24 Apr 2021 00:16:22 GMT
ENV ROS2_DISTRO=eloquent
# Sat, 24 Apr 2021 00:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.10-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:20:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.3-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:21:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6301496ad88f969ba47c05899ce2574e868ece07476fa3d1addbbaeead7fb068`  
		Last Modified: Fri, 23 Apr 2021 22:40:02 GMT  
		Size: 22.3 MB (22292158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3c5f836c0e7b3c6da7e297558c3db50e9103f5bab852ac45dfbd4fff190497`  
		Last Modified: Fri, 23 Apr 2021 22:39:57 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815a8cb3d4b6de76a6fe9c5945ba5e5f898c24e70d5160317fcd7739f758508`  
		Last Modified: Fri, 23 Apr 2021 22:39:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d75883e56f343cacf3b5820edf4672f0fc1357c53cb0f1390d1c1600271fd6`  
		Last Modified: Sat, 24 Apr 2021 00:28:33 GMT  
		Size: 841.3 KB (841296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984c57909785a02292fb5bdd227624764e91ad4ac971c6448b75895e6524abdf`  
		Last Modified: Sat, 24 Apr 2021 00:28:30 GMT  
		Size: 4.1 MB (4085739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2858eede13d67857768c9517993a7e6243252725b7e1e8d99de000c4e96cbe`  
		Last Modified: Sat, 24 Apr 2021 00:28:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0620a8195483bac3f3962b12fc3857bcc59b467d13f922afc2d67201ea17a6c4`  
		Last Modified: Sat, 24 Apr 2021 00:42:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3f57960bca3e9c5fc604feff70660d14bc82622913989ef87bced397dbbbe`  
		Last Modified: Sat, 24 Apr 2021 00:47:57 GMT  
		Size: 156.6 MB (156603123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab7b9c377dd46e5fd5a000001e40139b2a2eccacb164782de5abfa0ee3fe60e`  
		Last Modified: Sat, 24 Apr 2021 00:46:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90de6de82e4ed98837e99f3fed2d57cccb1583e87bcde6e36e6fa059fe9ce33c`  
		Last Modified: Sat, 24 Apr 2021 00:48:25 GMT  
		Size: 47.9 MB (47921382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccae62ac4ec4d945ca70973bb739c657fa9dc16cbb8bcbe1414278e751ddc3f`  
		Last Modified: Sat, 24 Apr 2021 00:48:07 GMT  
		Size: 205.4 KB (205391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daff81c507a6eb92c36f893b3a6771b1c87dd69f85799349cee101f7ddcf6e7`  
		Last Modified: Sat, 24 Apr 2021 00:48:10 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c7c79a04d873d9d31b5b215b8cf43626b89b308c8b675f3d93355a0778d1e8`  
		Last Modified: Sat, 24 Apr 2021 00:48:14 GMT  
		Size: 3.5 MB (3496932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07438edf58032ffe861153d2fd5de4039ec8029b346ab2448520605962d3e940`  
		Last Modified: Sat, 24 Apr 2021 00:48:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1644d2ad1461da49ede207a50b679a056267607e671fc028fd30d850f09079`  
		Last Modified: Sat, 24 Apr 2021 00:48:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f845622f4b00f581478e53a7aa307ba0ae6c4fffc293e9dfc9a8684726b2a4`  
		Last Modified: Sat, 24 Apr 2021 00:49:37 GMT  
		Size: 110.6 MB (110645934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d943ada60e24ee47d625b99474785e6d3aab079f75d02b14e329b1cb7cd7dda`  
		Last Modified: Sat, 24 Apr 2021 00:49:23 GMT  
		Size: 82.2 MB (82221660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe2427a3a435c47775238a90ada2f54c82f258c4220c7af9a4fc5f538d169ea`  
		Last Modified: Sat, 24 Apr 2021 00:48:35 GMT  
		Size: 734.0 KB (734018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc799a5a35341cc55ca3431d486b108089742f34408ac137219fd988722e3d48`  
		Last Modified: Sat, 24 Apr 2021 00:48:35 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eac8ee12538a3fcc76fa9eb539ae381fbb206fd65bdb424c23ee67ccb0367ea3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **464.1 MB (464098609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d6ec1ee3f19382bdc9cd5eaddc6f0bf67072425d9e9bdb2b44c22618ec2909`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:23:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:23:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:23:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 00:46:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 24 Apr 2021 00:46:17 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 00:46:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 24 Apr 2021 00:53:59 GMT
ENV ROS_DISTRO=eloquent
# Sat, 24 Apr 2021 00:56:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:56:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 24 Apr 2021 00:56:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 00:56:54 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 00:57:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:58:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 00:58:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 24 Apr 2021 00:58:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:58:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 00:59:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 00:59:01 GMT
ENV ROS1_DISTRO=melodic
# Sat, 24 Apr 2021 00:59:03 GMT
ENV ROS2_DISTRO=eloquent
# Sat, 24 Apr 2021 01:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.10-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.3-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:03:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:03:18 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4d7949f503cfae35d1e4072cc9f714f7f8080ddc5b9c1a01a837bd00682493`  
		Last Modified: Sat, 24 Apr 2021 01:23:29 GMT  
		Size: 841.2 KB (841190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ffbacc392e75d546f657a3c5ccfb65077a82acaaf78fd4ee3e380b95ef811f`  
		Last Modified: Sat, 24 Apr 2021 01:23:26 GMT  
		Size: 4.5 MB (4453794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476ab02969bb3ddd3e04ec5657467e4e747f59f5e3e02c4af893ad380c8c6cfb`  
		Last Modified: Sat, 24 Apr 2021 01:23:23 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2ca8bca9319a705f62ad9a055c3c031669e45715063fe23a399dc70e087705`  
		Last Modified: Sat, 24 Apr 2021 01:34:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb1f6ada61ac221f57749e9f46fdfe5c1a1a0d49da126542cc2434a7792ba4`  
		Last Modified: Sat, 24 Apr 2021 01:38:42 GMT  
		Size: 168.4 MB (168402022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b6099d852cf1da33eb73a465970abde3c79d1e51a4fa4eec2cc7e8a058d4b6`  
		Last Modified: Sat, 24 Apr 2021 01:37:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744c53d7aefc9c91aabbc30fdd92193df3c8b7aac6fd0ad7c9a2a40e547292ad`  
		Last Modified: Sat, 24 Apr 2021 01:39:12 GMT  
		Size: 56.2 MB (56235806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efd49999485e38f34d9c9b46f32111535bf1a7f919ac7873a55d1f4cf95c640`  
		Last Modified: Sat, 24 Apr 2021 01:38:53 GMT  
		Size: 205.4 KB (205396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30cff8ca3052845ea796d06c11e9b1edd7bc919fe5aade7b0a884097b9293de`  
		Last Modified: Sat, 24 Apr 2021 01:38:53 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdede3460b6a3f04a43ca08d5e9a17b13da2ef2af1b8e5c3423fd5e0d765a7be`  
		Last Modified: Sat, 24 Apr 2021 01:38:59 GMT  
		Size: 3.9 MB (3935301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc78b7d6308bcba20f5ccfb01820d17296ce51069bba0f3401725e709b8c8f9d`  
		Last Modified: Sat, 24 Apr 2021 01:39:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53dab10f962a9fce00d2e99d36e60937cdace7ff227d9ebd43ac3f96e19bb163`  
		Last Modified: Sat, 24 Apr 2021 01:39:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb6f90603d660c1ad5ff1a84c98ea37a3b848363e3ebc3889fa57b979815679`  
		Last Modified: Sat, 24 Apr 2021 01:41:07 GMT  
		Size: 116.7 MB (116718273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a19ae9308c5addef91d7d2b30ba068c80c6e211dd7881880aa6cce0af422455`  
		Last Modified: Sat, 24 Apr 2021 01:40:52 GMT  
		Size: 88.9 MB (88861432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0166dfd389f2a5c48c1233ea0ba6c46ae283faba99b36189b3cc2051c72e9948`  
		Last Modified: Sat, 24 Apr 2021 01:39:22 GMT  
		Size: 736.1 KB (736138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89658c8e4c31b5438f19e581d8ffb69010f5765a09cb43557ca7405f906602a2`  
		Last Modified: Sat, 24 Apr 2021 01:39:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
