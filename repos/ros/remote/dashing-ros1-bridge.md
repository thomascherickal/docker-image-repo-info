## `ros:dashing-ros1-bridge`

```console
$ docker pull ros@sha256:fdd07275284634847643641e4590c640111e9e3b2e3172a1afd5dd9ae28c633e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:ac66eaacfb2df1ecbf5cce1f969bbb896171f603c61c16fc18343b0d53bf4ed3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **418.7 MB (418728483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ce5f280e14c0bbc889aaeb1fda33cb7755e96035f68f6c4cc6d25cbd316826`
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
# Sat, 24 Apr 2021 01:42:32 GMT
ENV ROS_DISTRO=dashing
# Sat, 24 Apr 2021 01:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:45:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 24 Apr 2021 01:45:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 01:45:10 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 01:46:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:46:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 01:46:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 24 Apr 2021 01:46:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 01:46:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 01:46:41 GMT
ENV ROS1_DISTRO=melodic
# Sat, 24 Apr 2021 01:46:41 GMT
ENV ROS2_DISTRO=dashing
# Sat, 24 Apr 2021 01:49:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.10-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:49:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.8-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:49:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:49:27 GMT
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
	-	`sha256:ef225211becc9ab6071ae7cc9f7ac6048bf6a18245b84cec9f6b04ea919f1b3e`  
		Last Modified: Sat, 24 Apr 2021 02:12:06 GMT  
		Size: 179.4 MB (179425960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc82edab3cea6ebc843bae806b3a9c489685d0d46333ddeba0ceaa91bfbc18e4`  
		Last Modified: Sat, 24 Apr 2021 02:11:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870d69149c1594db53b0cdbabcef095fa512cbedfe1d1ee466ba8387c68af45e`  
		Last Modified: Sat, 24 Apr 2021 02:12:29 GMT  
		Size: 64.2 MB (64159458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460921d156edc29363cc23e1785c3ab00163de798e72cfd806de4daabfb9e67a`  
		Last Modified: Sat, 24 Apr 2021 02:12:19 GMT  
		Size: 206.7 KB (206692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9a9815b6cce336221f3813bfcf47b90d3e732914daba851b15d830e3c53092`  
		Last Modified: Sat, 24 Apr 2021 02:12:18 GMT  
		Size: 2.0 KB (2021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3460c248fe6f2a070b013eede5d78f2b7f327a169abbf1ff0d7e16ba71e6c`  
		Last Modified: Sat, 24 Apr 2021 02:12:20 GMT  
		Size: 4.3 MB (4315291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72ce8992bf9b925ee3148b5ad6241fd2ef67f86214d6ec5952248dc148683e0`  
		Last Modified: Sat, 24 Apr 2021 02:12:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270739a9c0638aec85b0e377d96e9cfd72fecba3726adf88b39149b00d47bc04`  
		Last Modified: Sat, 24 Apr 2021 02:12:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c7ea997c4bdf7140b3da57d3ced6ca8b45c7d6ce18666801856c76c247286a`  
		Last Modified: Sat, 24 Apr 2021 02:13:08 GMT  
		Size: 117.8 MB (117759480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d55aa8f46d8c910ecdb0ce6edc00b5d6a426f505fb330a3c8b30d295f97f618`  
		Last Modified: Sat, 24 Apr 2021 02:12:49 GMT  
		Size: 19.8 MB (19803809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b5625bcb4986e4ee836130c74aaf7c2cc8aab66f2904fe6d9c42176bb213f5`  
		Last Modified: Sat, 24 Apr 2021 02:12:44 GMT  
		Size: 640.4 KB (640356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b71ea10bdddb8bf347cebaf4479cbd9874673a1a6d8364dbdc01e95da679e83`  
		Last Modified: Sat, 24 Apr 2021 02:12:44 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:a29accb36aec8b8d1ef736f265907b34ac23af92aef1c6098ef5dd6c3ca1d853
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354874293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c010ee255f32f8c59a414db52c54a1a00cd31bc8abdee12106c0ec6b67a2501`
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
# Fri, 23 Apr 2021 23:58:26 GMT
ENV ROS_DISTRO=dashing
# Sat, 24 Apr 2021 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:01:21 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 24 Apr 2021 00:01:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 00:01:28 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 00:02:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 00:03:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 24 Apr 2021 00:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:04:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 00:04:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 00:04:58 GMT
ENV ROS1_DISTRO=melodic
# Sat, 24 Apr 2021 00:05:04 GMT
ENV ROS2_DISTRO=dashing
# Sat, 24 Apr 2021 00:08:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.10-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:08:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.8-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:09:14 GMT
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
	-	`sha256:5ce9092f388405fc16016eafbeda696f841295a9c1a8f48e26c9107297531275`  
		Last Modified: Sat, 24 Apr 2021 00:43:54 GMT  
		Size: 153.6 MB (153552668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8de250b90a2ccfda462770b28a23df457b26782ce432e2219e9085b3313639`  
		Last Modified: Sat, 24 Apr 2021 00:42:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a23889664fc8f33d2f2abe2106e228c5a0c8313d8d3e19f540b786d82090513`  
		Last Modified: Sat, 24 Apr 2021 00:44:26 GMT  
		Size: 48.5 MB (48549613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2105f6b512e7e83f147bcb946a99bbf44a45626fbcf3065efd7be75a7f8e6859`  
		Last Modified: Sat, 24 Apr 2021 00:44:02 GMT  
		Size: 206.7 KB (206699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127df38c0ca62dd908b74f5cbb4e77523caa8c713485d8b3c2cf3333459c6d5`  
		Last Modified: Sat, 24 Apr 2021 00:44:02 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e495e5412ffd2cf67e790ec102d0a3d969d74d26f7335bfce35a9326bf34ba10`  
		Last Modified: Sat, 24 Apr 2021 00:44:13 GMT  
		Size: 3.3 MB (3250409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b8d431c225ddde27f5e14aad1fd9cbb7df38cf2c59b72a4e913e7996fa9311`  
		Last Modified: Sat, 24 Apr 2021 00:44:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99801588fc860ae7c2f5d903f4e37fc4d27fa92987a597b0fae06f16d017345`  
		Last Modified: Sat, 24 Apr 2021 00:44:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8bb3d71e764af2aa3798779475056709119daef25a936010b1392651bcd4b0`  
		Last Modified: Sat, 24 Apr 2021 00:46:15 GMT  
		Size: 110.6 MB (110639503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba274063dccd1d4fc63c86825efd4487acafc45d13f431936db9ab148fde823d`  
		Last Modified: Sat, 24 Apr 2021 00:44:58 GMT  
		Size: 10.8 MB (10814591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209bd6cc0362f11c289dee526d386c22926acb85565cc4d26c6abbf1a8056fb`  
		Last Modified: Sat, 24 Apr 2021 00:44:35 GMT  
		Size: 636.1 KB (636063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881e97cc946a2e60ea50f7d6b19adfdfcbd14460f677f3c7af0035d32576100b`  
		Last Modified: Sat, 24 Apr 2021 00:44:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c2ddd77afef77b308964f6fb0d68d5f9726a604a9c4a9b6104229aa22678ffd2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.1 MB (387128306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf634b9f0b70a0144fe7da2d5539241136623bced36b8dca39de70a79e87bf08`
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
# Sat, 24 Apr 2021 00:46:20 GMT
ENV ROS_DISTRO=dashing
# Sat, 24 Apr 2021 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:48:34 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 24 Apr 2021 00:48:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 00:48:37 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 00:49:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:49:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 00:50:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 24 Apr 2021 00:50:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:50:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 24 Apr 2021 00:50:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 00:50:46 GMT
ENV ROS1_DISTRO=melodic
# Sat, 24 Apr 2021 00:50:47 GMT
ENV ROS2_DISTRO=dashing
# Sat, 24 Apr 2021 00:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.10-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:53:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.8-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:53:50 GMT
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
	-	`sha256:5adf08fb5b90b52af6b256933f72b2da13942e3ade84fb585ea596819f75fdf2`  
		Last Modified: Sat, 24 Apr 2021 01:35:26 GMT  
		Size: 165.1 MB (165084725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77055f56a634a7319b39c0385893dbd785dc118c58eff975f1580d46b47bc19`  
		Last Modified: Sat, 24 Apr 2021 01:34:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c53ada37d4c6a81cc4f5fd4293c3df78e2beaab28d22dc76253817b676df7a`  
		Last Modified: Sat, 24 Apr 2021 01:35:56 GMT  
		Size: 56.9 MB (56860195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c964a93383c7e58d3d2fb154aec603556d5dbcacb788171e9d8e72a0548878`  
		Last Modified: Sat, 24 Apr 2021 01:35:33 GMT  
		Size: 206.7 KB (206704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce2412f05de9a243f5c07fba71293b71ad9ffa629dfb97b422181d3f2cf1a2f`  
		Last Modified: Sat, 24 Apr 2021 01:35:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c8fc9cd612be15440372f1cfea322ee3af66c7bae68e78e8582bbf28079939`  
		Last Modified: Sat, 24 Apr 2021 01:35:38 GMT  
		Size: 3.7 MB (3665919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33524add0779ac951085f92c5935858a9115b757da3f284ccc2c06a6f81b7f53`  
		Last Modified: Sat, 24 Apr 2021 01:36:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3640644db357d9796a32f7b688654cbaaf2c446b20c9ddec8642cff030a789`  
		Last Modified: Sat, 24 Apr 2021 01:36:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a26af9c561918a6c19f2c60de252e930af7b2e024f0d99a8fa5accfc0a659b`  
		Last Modified: Sat, 24 Apr 2021 01:37:31 GMT  
		Size: 116.7 MB (116710790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beddfafc6ff3fe5ebb94b1cf439041beec0bafe2dbd5ba9fa723a51de86f11ec`  
		Last Modified: Sat, 24 Apr 2021 01:36:29 GMT  
		Size: 15.0 MB (14958419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c06cb18cb2f8dc46cb03c322a30ea54ff477cc51a29e0ecd9133eaf17b8b75`  
		Last Modified: Sat, 24 Apr 2021 01:36:08 GMT  
		Size: 637.3 KB (637313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612f3ef1ce46744309816e491423e88b11a9b9b4bcac9035b2cd35d8cb0ee90`  
		Last Modified: Sat, 24 Apr 2021 01:36:10 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
