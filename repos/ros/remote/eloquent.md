## `ros:eloquent`

```console
$ docker pull ros@sha256:1a678c792fa69d28aec5e52d9b387b869c27e9d2f4916a47899adf162fab6aa9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent` - linux; amd64

```console
$ docker pull ros@sha256:87138e798839389ead278e98f829fcbf76e5584c6bd9dfb82319b24c768f96af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283652405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75f02804aa2a26a5cf776c9eba5789b9985529334fd827d09e21aa510ac4121`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Tue, 19 May 2020 18:27:41 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:29:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:29:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 May 2020 00:45:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 27 May 2020 00:45:30 GMT
ENV LANG=C.UTF-8
# Wed, 27 May 2020 00:45:31 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 May 2020 00:48:35 GMT
ENV ROS_DISTRO=eloquent
# Wed, 27 May 2020 00:49:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:49:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 27 May 2020 00:49:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 May 2020 00:49:42 GMT
CMD ["bash"]
# Wed, 27 May 2020 00:50:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:50:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 27 May 2020 00:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 27 May 2020 00:50:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1fb7c1137ce366c52ed0850f79d5d96e24ecd02d5e5a6692c4265203713bdd`  
		Last Modified: Tue, 19 May 2020 18:53:24 GMT  
		Size: 837.5 KB (837516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6481f53850f8302d04fa37826e23bd91669bb22244764a2378bc03775063b3c0`  
		Last Modified: Wed, 27 May 2020 00:53:51 GMT  
		Size: 4.9 MB (4867298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d033e4703843b0f18fa16f9373153855816f953158e199abd64dec4a381abefe`  
		Last Modified: Wed, 27 May 2020 00:53:51 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf4d671437c6cca9ed496889014b8140ef23f5c4675b72c0d0fe9efba15e7dc`  
		Last Modified: Wed, 27 May 2020 00:59:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e4c78a58a8cdfb263c587166a2b930c1d53673bca56eb45d4b4afd79338761`  
		Last Modified: Wed, 27 May 2020 01:00:47 GMT  
		Size: 183.0 MB (182957709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1cad8723eacfa2d0ec00f5121385cee0dac2ba73a9d429c347f35dc859a3c3`  
		Last Modified: Wed, 27 May 2020 01:00:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ec2ac3fcf05e34c021cbf90b62a823ea912bf2f1ac3c18444149d780355b`  
		Last Modified: Wed, 27 May 2020 01:01:05 GMT  
		Size: 63.5 MB (63500557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85574b1744cfd307dddc376eaf3e849367780593f2d8039c534ff7ffec527ffb`  
		Last Modified: Wed, 27 May 2020 01:00:52 GMT  
		Size: 179.7 KB (179664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf79a49ec131fd66dae597908753089f7ba7d99049d2299d0aedb037e351e5`  
		Last Modified: Wed, 27 May 2020 01:00:51 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7abdb4129b638087780dd976c24acde6b7b241a5dfa9343a7bd590a60d3c5ca`  
		Last Modified: Wed, 27 May 2020 01:00:53 GMT  
		Size: 4.6 MB (4579649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm variant v7

```console
$ docker pull ros@sha256:2cb3b910deb192ca591badccdd15a4c27628915474bfb7a8f9cf93e6d5479f32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241928720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ee092821a3309f339fc27d1c67a3c434427f05708d245edf3294b7e605a426`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:06:03 GMT
ADD file:7b716521aeb6ae372a2660a2e5fc6c55001a12772c5f808963363b3194c1b6f1 in / 
# Thu, 23 Apr 2020 22:06:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 22:06:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:06:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:06:12 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:40:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:52:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:52:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:52:47 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 11:53:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:53:45 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:53:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:56:04 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 11:56:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:56:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 11:56:24 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 11:57:41 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:57:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 11:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:57:45 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:58:08 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfb2710e7a499e5a0ecb4a694f4ec66c08a8a7501cdd43d1bcef61a54ca008b8`  
		Last Modified: Sun, 05 Apr 2020 20:24:11 GMT  
		Size: 22.3 MB (22276244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78424bd0db4f26216c80c16f14cdbb94424732ed34e91c84303d4e9fe2a819a`  
		Last Modified: Thu, 23 Apr 2020 22:08:18 GMT  
		Size: 35.5 KB (35463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60330e98a48fe01f9fadb99c597930437c15e1a00006e43234404e20d5e5471b`  
		Last Modified: Thu, 23 Apr 2020 22:08:18 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc5290c7dcf9b435262d02bb531959de9b08c5cc139b9ea46fda8061af60116`  
		Last Modified: Thu, 23 Apr 2020 22:08:18 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1ceaaa3e19542e3d9df84a96b053318b0aa21a68a6eb8f81aa613aabbc79bb`  
		Last Modified: Fri, 24 Apr 2020 12:01:59 GMT  
		Size: 838.5 KB (838503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361c104ad16f1ead25264ba3fcc969959c55179c23b5c8a8c039797d3e5f3b8b`  
		Last Modified: Fri, 24 Apr 2020 12:06:16 GMT  
		Size: 138.5 MB (138458606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a11353a3d4af5e2f00b0bb31bf18be3c591c91f514de5d0b4abb8953dd60368`  
		Last Modified: Fri, 24 Apr 2020 12:05:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17a60943588ae237ec24134142f427463ef1241d8c64e4512d3bfe96b8249da`  
		Last Modified: Fri, 24 Apr 2020 12:05:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a23d42ea431ab542285d19fb2bb2956875c21bcf0930bbac54463888429c5e`  
		Last Modified: Fri, 24 Apr 2020 12:05:54 GMT  
		Size: 33.7 MB (33682827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e740f7ac7081d7745b5562c69cf403a03e1fa6f5af96f11f217c4e0718cf70a`  
		Last Modified: Fri, 24 Apr 2020 12:06:39 GMT  
		Size: 175.6 KB (175616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f9d28d53f0b96c6a55b23e7d17576f74fe8c7bf75cf47b6500d3b38ac1c3c`  
		Last Modified: Fri, 24 Apr 2020 12:06:39 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea24a3be1fd22ccd2ba469813d232a241cdf76537ace576dcb9b2470900d8949`  
		Last Modified: Fri, 24 Apr 2020 12:06:39 GMT  
		Size: 210.0 KB (209975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b22b1e784cd59314a7ad24c84b5aeacc740f206b73e115bf57b7e4d004c06`  
		Last Modified: Fri, 24 Apr 2020 12:06:55 GMT  
		Size: 42.7 MB (42729607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b8ca32f38d3833cadd835df28eb753a4c4745a34e55c0d6b62b9f30df0f6ef`  
		Last Modified: Fri, 24 Apr 2020 12:06:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b50131ae3fa4ea4eb94c5a3a8c858a529c0701e35a092e07c867d3c954bc8d7`  
		Last Modified: Fri, 24 Apr 2020 12:07:06 GMT  
		Size: 3.5 MB (3517009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5aba46e2ad3e90b20283263075e6c7e5c9c035ce52dfbf1efeebd5eb323c7e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.3 MB (264340441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c024ffa21ff8f19dc56c499417dd3d98818a40a89c30399624592dcab58c52b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:17:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:32:45 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:32:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:32:56 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 15:33:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:33:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:33:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:36:09 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 15:36:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:36:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 15:36:29 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 15:37:59 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:38:03 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 15:38:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:38:04 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:38:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6109c4847aeddf3d64c15cc74fbb9b3ba8594f1313612a07a0b5b8ae6560d3e`  
		Last Modified: Fri, 24 Apr 2020 15:42:12 GMT  
		Size: 837.9 KB (837905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af28e356225383804f77c94dd71b6c3f2e5194cefcdd7ed8bb9fa2ff7f8684b`  
		Last Modified: Fri, 24 Apr 2020 15:46:21 GMT  
		Size: 150.7 MB (150721265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e32aa202b67c818326cf3212a9131e926e01f8bf3d01b49e3be9e9aca81a91`  
		Last Modified: Fri, 24 Apr 2020 15:45:45 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3873286145cc87cfd355db790697e93051a620dd413e8d4ee85557170478bc89`  
		Last Modified: Fri, 24 Apr 2020 15:45:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73278ce1f1ce19f125b788107f697cb09bfb9757e5b69efe0a122ce013b2f90`  
		Last Modified: Fri, 24 Apr 2020 15:45:56 GMT  
		Size: 36.5 MB (36476048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254243c190cb0033848dd1fc526a8bb4faa5cd8999bf6d4b6d9d20c95b84a6c2`  
		Last Modified: Fri, 24 Apr 2020 15:46:37 GMT  
		Size: 175.6 KB (175622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e91133eaf611b6724b5f51b5449e2217384043a45f5de233c7d843142a4d46`  
		Last Modified: Fri, 24 Apr 2020 15:46:37 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e3ca04048d46857eebbc29bf7ab3c441c38c81dbca181ba245cb49ce243272`  
		Last Modified: Fri, 24 Apr 2020 15:46:37 GMT  
		Size: 209.9 KB (209931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a351b4c664b3b4814456e1c6474b7c774c3736660cb399aee33ba1f973cb028`  
		Last Modified: Fri, 24 Apr 2020 15:46:54 GMT  
		Size: 48.2 MB (48203962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4431967b3623e79ef33a679c7eb9809cfbb086b1df2c5d090666265f08819732`  
		Last Modified: Fri, 24 Apr 2020 15:46:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74c79a8b8286b0e14b8f818a40a026d935ec1e41974f48b672ae2c25bff748e`  
		Last Modified: Fri, 24 Apr 2020 15:47:01 GMT  
		Size: 4.0 MB (3955246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
