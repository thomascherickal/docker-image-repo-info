<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:dashing`](#rosdashing)
-	[`ros:dashing-ros-base`](#rosdashing-ros-base)
-	[`ros:dashing-ros-base-bionic`](#rosdashing-ros-base-bionic)
-	[`ros:dashing-ros-core`](#rosdashing-ros-core)
-	[`ros:dashing-ros-core-bionic`](#rosdashing-ros-core-bionic)
-	[`ros:eloquent`](#roseloquent)
-	[`ros:eloquent-ros-base`](#roseloquent-ros-base)
-	[`ros:eloquent-ros-base-bionic`](#roseloquent-ros-base-bionic)
-	[`ros:eloquent-ros-core`](#roseloquent-ros-core)
-	[`ros:eloquent-ros-core-bionic`](#roseloquent-ros-core-bionic)
-	[`ros:kinetic`](#roskinetic)
-	[`ros:kinetic-perception`](#roskinetic-perception)
-	[`ros:kinetic-perception-xenial`](#roskinetic-perception-xenial)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-robot-xenial`](#roskinetic-robot-xenial)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic-ros-base-xenial`](#roskinetic-ros-base-xenial)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-core-xenial`](#roskinetic-ros-core-xenial)
-	[`ros:latest`](#roslatest)
-	[`ros:melodic`](#rosmelodic)
-	[`ros:melodic-perception`](#rosmelodic-perception)
-	[`ros:melodic-perception-bionic`](#rosmelodic-perception-bionic)
-	[`ros:melodic-perception-stretch`](#rosmelodic-perception-stretch)
-	[`ros:melodic-robot`](#rosmelodic-robot)
-	[`ros:melodic-robot-bionic`](#rosmelodic-robot-bionic)
-	[`ros:melodic-robot-stretch`](#rosmelodic-robot-stretch)
-	[`ros:melodic-ros-base`](#rosmelodic-ros-base)
-	[`ros:melodic-ros-base-bionic`](#rosmelodic-ros-base-bionic)
-	[`ros:melodic-ros-base-stretch`](#rosmelodic-ros-base-stretch)
-	[`ros:melodic-ros-core`](#rosmelodic-ros-core)
-	[`ros:melodic-ros-core-bionic`](#rosmelodic-ros-core-bionic)
-	[`ros:melodic-ros-core-stretch`](#rosmelodic-ros-core-stretch)

## `ros:dashing`

```console
$ docker pull ros@sha256:37f91f752c1a54e01840fd44369cbb303188257fd16290a9cd243a096b53872b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing` - linux; amd64

```console
$ docker pull ros@sha256:b817b698c95ece32712f3efac2969c8861adc8d209479fa94e1485a0ab0bccc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.9 MB (287878887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ce86a874d29c4dcba32a1bec9c432a8fb7206e4a9e99ff134849bb7d809532`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:07:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 21:08:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:08:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:08:05 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:08:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:08:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:08:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:08:47 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:08:59 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201572245620c3000c316fd1492239ba1b53dde9404e8ad4898ad3ad5149d0a`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 177.3 KB (177335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528594ff3960aa89cd0da4c3dceff027b23e8aa79f131d87885c336fb8a89a9`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 1.9 KB (1933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991516221b05d87cc9aa98a4a73f10a169e4a33f47497712fc27858013debe1`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 209.6 KB (209601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c0aa22f0eed42b3091e88dd92fe1f057ba3031c66338b643ff1945078f33fd`  
		Last Modified: Fri, 24 Apr 2020 21:16:11 GMT  
		Size: 58.7 MB (58669093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58ce7d77b31e6816ff071ce4bc528276c2c3013b2ee8b0034bd59b73e41d1ec`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748be1a32598ecfdf0cc3e77bead485d9530032302ff86cbdc4974a4845120bd`  
		Last Modified: Fri, 24 Apr 2020 21:16:25 GMT  
		Size: 4.3 MB (4339582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm variant v7

```console
$ docker pull ros@sha256:8c04caf2904141ec529b76e15205817fd862e9895d0a9a56638dff67770bf064
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.9 MB (239923740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d022d2e2971478395f681fb67e37643c8370b77cc927d8ea3eae5689e7950494`
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
# Fri, 24 Apr 2020 11:53:46 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 11:53:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:54:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 11:54:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 11:55:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:55:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 11:55:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:55:30 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:55:56 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0bad75f33094b614b5bfa5655ddce2210323fb7103d02c9ed57e106baf650cf8`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 177.4 KB (177405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba9633ff2ebf9b850124a9eba586560dfebd225ce62f80388bf42b2a9bc99c`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3306e3aac3a99c454ebf90e8b2cb79752be4ebdfab9a9dd70f49efb235db34c0`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 210.0 KB (209993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d28731e7682f5988588065df3ee6c605004ef8398946cde0ead6f713f1a28`  
		Last Modified: Fri, 24 Apr 2020 12:05:57 GMT  
		Size: 41.0 MB (40961944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8549512425231a158ecb89db00bc97fddf3fab27a4d2e03049fbed925e9435ec`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875215957d77291941aa0786e6933d662e26f3a83a060ec759feae208e4c5dfe`  
		Last Modified: Fri, 24 Apr 2020 12:06:27 GMT  
		Size: 3.3 MB (3277895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:887833e32b2016c75a76b08a33b7ff95f07697c45b58593fac90a3448be9f92d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.1 MB (262054198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:688957a4145f9d565cbfd8219ddc81936a1c96dfbe34402b9702ea1ef549795f`
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
# Fri, 24 Apr 2020 15:33:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 15:34:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:34:11 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 15:34:16 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 15:35:30 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:35:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 15:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:35:34 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:36:02 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:168853c0e5c582a7986b59314f3ce5c2ab47f8f2a9d9347f9cca1093e0194b71`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 177.4 KB (177400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1710afaf7ca4719abefac326d77752a6db0f8f43b44924bde460a4b5b179bc39`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85f2813ff6412bbb7db99536c8ec0cc3ae6d08b37c6d3a9c262cac96f44cf7`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 209.9 KB (209922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a01ecfb5685d76a60d5a301aaf7a4e7b7ef43c49c1be7999f005023a4036`  
		Last Modified: Fri, 24 Apr 2020 15:46:02 GMT  
		Size: 46.2 MB (46179126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0599aa73709e9fd4f80ef366250b76286573192a77ae03cf2729835ddee1d`  
		Last Modified: Fri, 24 Apr 2020 15:45:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51191614b9fdfda20e22f0d5976b9a09b67b44a72ee5027d0e90f5fd159213d`  
		Last Modified: Fri, 24 Apr 2020 15:46:30 GMT  
		Size: 3.7 MB (3692080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base`

```console
$ docker pull ros@sha256:37f91f752c1a54e01840fd44369cbb303188257fd16290a9cd243a096b53872b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b817b698c95ece32712f3efac2969c8861adc8d209479fa94e1485a0ab0bccc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.9 MB (287878887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ce86a874d29c4dcba32a1bec9c432a8fb7206e4a9e99ff134849bb7d809532`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:07:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 21:08:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:08:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:08:05 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:08:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:08:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:08:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:08:47 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:08:59 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201572245620c3000c316fd1492239ba1b53dde9404e8ad4898ad3ad5149d0a`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 177.3 KB (177335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528594ff3960aa89cd0da4c3dceff027b23e8aa79f131d87885c336fb8a89a9`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 1.9 KB (1933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991516221b05d87cc9aa98a4a73f10a169e4a33f47497712fc27858013debe1`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 209.6 KB (209601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c0aa22f0eed42b3091e88dd92fe1f057ba3031c66338b643ff1945078f33fd`  
		Last Modified: Fri, 24 Apr 2020 21:16:11 GMT  
		Size: 58.7 MB (58669093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58ce7d77b31e6816ff071ce4bc528276c2c3013b2ee8b0034bd59b73e41d1ec`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748be1a32598ecfdf0cc3e77bead485d9530032302ff86cbdc4974a4845120bd`  
		Last Modified: Fri, 24 Apr 2020 21:16:25 GMT  
		Size: 4.3 MB (4339582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:8c04caf2904141ec529b76e15205817fd862e9895d0a9a56638dff67770bf064
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.9 MB (239923740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d022d2e2971478395f681fb67e37643c8370b77cc927d8ea3eae5689e7950494`
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
# Fri, 24 Apr 2020 11:53:46 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 11:53:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:54:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 11:54:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 11:55:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:55:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 11:55:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:55:30 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:55:56 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0bad75f33094b614b5bfa5655ddce2210323fb7103d02c9ed57e106baf650cf8`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 177.4 KB (177405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba9633ff2ebf9b850124a9eba586560dfebd225ce62f80388bf42b2a9bc99c`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3306e3aac3a99c454ebf90e8b2cb79752be4ebdfab9a9dd70f49efb235db34c0`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 210.0 KB (209993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d28731e7682f5988588065df3ee6c605004ef8398946cde0ead6f713f1a28`  
		Last Modified: Fri, 24 Apr 2020 12:05:57 GMT  
		Size: 41.0 MB (40961944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8549512425231a158ecb89db00bc97fddf3fab27a4d2e03049fbed925e9435ec`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875215957d77291941aa0786e6933d662e26f3a83a060ec759feae208e4c5dfe`  
		Last Modified: Fri, 24 Apr 2020 12:06:27 GMT  
		Size: 3.3 MB (3277895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:887833e32b2016c75a76b08a33b7ff95f07697c45b58593fac90a3448be9f92d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.1 MB (262054198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:688957a4145f9d565cbfd8219ddc81936a1c96dfbe34402b9702ea1ef549795f`
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
# Fri, 24 Apr 2020 15:33:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 15:34:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:34:11 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 15:34:16 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 15:35:30 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:35:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 15:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:35:34 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:36:02 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:168853c0e5c582a7986b59314f3ce5c2ab47f8f2a9d9347f9cca1093e0194b71`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 177.4 KB (177400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1710afaf7ca4719abefac326d77752a6db0f8f43b44924bde460a4b5b179bc39`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85f2813ff6412bbb7db99536c8ec0cc3ae6d08b37c6d3a9c262cac96f44cf7`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 209.9 KB (209922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a01ecfb5685d76a60d5a301aaf7a4e7b7ef43c49c1be7999f005023a4036`  
		Last Modified: Fri, 24 Apr 2020 15:46:02 GMT  
		Size: 46.2 MB (46179126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0599aa73709e9fd4f80ef366250b76286573192a77ae03cf2729835ddee1d`  
		Last Modified: Fri, 24 Apr 2020 15:45:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51191614b9fdfda20e22f0d5976b9a09b67b44a72ee5027d0e90f5fd159213d`  
		Last Modified: Fri, 24 Apr 2020 15:46:30 GMT  
		Size: 3.7 MB (3692080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base-bionic`

```console
$ docker pull ros@sha256:37f91f752c1a54e01840fd44369cbb303188257fd16290a9cd243a096b53872b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b817b698c95ece32712f3efac2969c8861adc8d209479fa94e1485a0ab0bccc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.9 MB (287878887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ce86a874d29c4dcba32a1bec9c432a8fb7206e4a9e99ff134849bb7d809532`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:07:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 21:08:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:08:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:08:05 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:08:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:08:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:08:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:08:47 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:08:59 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201572245620c3000c316fd1492239ba1b53dde9404e8ad4898ad3ad5149d0a`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 177.3 KB (177335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528594ff3960aa89cd0da4c3dceff027b23e8aa79f131d87885c336fb8a89a9`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 1.9 KB (1933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991516221b05d87cc9aa98a4a73f10a169e4a33f47497712fc27858013debe1`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 209.6 KB (209601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c0aa22f0eed42b3091e88dd92fe1f057ba3031c66338b643ff1945078f33fd`  
		Last Modified: Fri, 24 Apr 2020 21:16:11 GMT  
		Size: 58.7 MB (58669093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58ce7d77b31e6816ff071ce4bc528276c2c3013b2ee8b0034bd59b73e41d1ec`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748be1a32598ecfdf0cc3e77bead485d9530032302ff86cbdc4974a4845120bd`  
		Last Modified: Fri, 24 Apr 2020 21:16:25 GMT  
		Size: 4.3 MB (4339582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:8c04caf2904141ec529b76e15205817fd862e9895d0a9a56638dff67770bf064
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.9 MB (239923740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d022d2e2971478395f681fb67e37643c8370b77cc927d8ea3eae5689e7950494`
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
# Fri, 24 Apr 2020 11:53:46 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 11:53:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:54:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 11:54:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 11:55:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:55:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 11:55:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:55:30 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:55:56 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0bad75f33094b614b5bfa5655ddce2210323fb7103d02c9ed57e106baf650cf8`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 177.4 KB (177405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba9633ff2ebf9b850124a9eba586560dfebd225ce62f80388bf42b2a9bc99c`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3306e3aac3a99c454ebf90e8b2cb79752be4ebdfab9a9dd70f49efb235db34c0`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 210.0 KB (209993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d28731e7682f5988588065df3ee6c605004ef8398946cde0ead6f713f1a28`  
		Last Modified: Fri, 24 Apr 2020 12:05:57 GMT  
		Size: 41.0 MB (40961944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8549512425231a158ecb89db00bc97fddf3fab27a4d2e03049fbed925e9435ec`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875215957d77291941aa0786e6933d662e26f3a83a060ec759feae208e4c5dfe`  
		Last Modified: Fri, 24 Apr 2020 12:06:27 GMT  
		Size: 3.3 MB (3277895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:887833e32b2016c75a76b08a33b7ff95f07697c45b58593fac90a3448be9f92d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.1 MB (262054198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:688957a4145f9d565cbfd8219ddc81936a1c96dfbe34402b9702ea1ef549795f`
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
# Fri, 24 Apr 2020 15:33:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 15:34:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:34:11 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 15:34:16 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 15:35:30 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:35:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 15:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:35:34 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:36:02 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:168853c0e5c582a7986b59314f3ce5c2ab47f8f2a9d9347f9cca1093e0194b71`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 177.4 KB (177400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1710afaf7ca4719abefac326d77752a6db0f8f43b44924bde460a4b5b179bc39`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85f2813ff6412bbb7db99536c8ec0cc3ae6d08b37c6d3a9c262cac96f44cf7`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 209.9 KB (209922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a01ecfb5685d76a60d5a301aaf7a4e7b7ef43c49c1be7999f005023a4036`  
		Last Modified: Fri, 24 Apr 2020 15:46:02 GMT  
		Size: 46.2 MB (46179126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0599aa73709e9fd4f80ef366250b76286573192a77ae03cf2729835ddee1d`  
		Last Modified: Fri, 24 Apr 2020 15:45:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51191614b9fdfda20e22f0d5976b9a09b67b44a72ee5027d0e90f5fd159213d`  
		Last Modified: Fri, 24 Apr 2020 15:46:30 GMT  
		Size: 3.7 MB (3692080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core`

```console
$ docker pull ros@sha256:e776749e71388f4506b580a2caa492b6d6fdadf5bf4324a2579dc60c0d5f20b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ba0099c87967ad3deca5640c926c7a8f103bc8ff530c6adf33e154781dc746b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283539305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65a68a3c2ad39fd1c5494952c099752a319159620f8655dda24c4c1174f9b0e1`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:07:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 21:08:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:08:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:08:05 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:08:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:08:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:08:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:08:47 GMT
CMD ["bash"]
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201572245620c3000c316fd1492239ba1b53dde9404e8ad4898ad3ad5149d0a`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 177.3 KB (177335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528594ff3960aa89cd0da4c3dceff027b23e8aa79f131d87885c336fb8a89a9`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 1.9 KB (1933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991516221b05d87cc9aa98a4a73f10a169e4a33f47497712fc27858013debe1`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 209.6 KB (209601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c0aa22f0eed42b3091e88dd92fe1f057ba3031c66338b643ff1945078f33fd`  
		Last Modified: Fri, 24 Apr 2020 21:16:11 GMT  
		Size: 58.7 MB (58669093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58ce7d77b31e6816ff071ce4bc528276c2c3013b2ee8b0034bd59b73e41d1ec`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:76c53e4c69a811901801a57d4cf1e50870e36e3c702642be5a8c60cce5a3a650
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236645845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2142ed3ab42e782e6ca0d450abae153237f4cd029b4f2c1279715ab180ef9f2`
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
# Fri, 24 Apr 2020 11:53:46 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 11:53:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:54:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 11:54:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 11:55:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:55:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 11:55:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:55:30 GMT
CMD ["bash"]
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
	-	`sha256:0bad75f33094b614b5bfa5655ddce2210323fb7103d02c9ed57e106baf650cf8`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 177.4 KB (177405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba9633ff2ebf9b850124a9eba586560dfebd225ce62f80388bf42b2a9bc99c`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3306e3aac3a99c454ebf90e8b2cb79752be4ebdfab9a9dd70f49efb235db34c0`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 210.0 KB (209993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d28731e7682f5988588065df3ee6c605004ef8398946cde0ead6f713f1a28`  
		Last Modified: Fri, 24 Apr 2020 12:05:57 GMT  
		Size: 41.0 MB (40961944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8549512425231a158ecb89db00bc97fddf3fab27a4d2e03049fbed925e9435ec`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a8c21cb4efdb75d6f650a101314069e762bd057fb05902927a0fa39166f722eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258362118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8375337e40a0dcf664a1f3991967dfbd082464f3a71de1c351032b99e4a064`
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
# Fri, 24 Apr 2020 15:33:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 15:34:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:34:11 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 15:34:16 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 15:35:30 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:35:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 15:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:35:34 GMT
CMD ["bash"]
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
	-	`sha256:168853c0e5c582a7986b59314f3ce5c2ab47f8f2a9d9347f9cca1093e0194b71`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 177.4 KB (177400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1710afaf7ca4719abefac326d77752a6db0f8f43b44924bde460a4b5b179bc39`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85f2813ff6412bbb7db99536c8ec0cc3ae6d08b37c6d3a9c262cac96f44cf7`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 209.9 KB (209922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a01ecfb5685d76a60d5a301aaf7a4e7b7ef43c49c1be7999f005023a4036`  
		Last Modified: Fri, 24 Apr 2020 15:46:02 GMT  
		Size: 46.2 MB (46179126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0599aa73709e9fd4f80ef366250b76286573192a77ae03cf2729835ddee1d`  
		Last Modified: Fri, 24 Apr 2020 15:45:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core-bionic`

```console
$ docker pull ros@sha256:e776749e71388f4506b580a2caa492b6d6fdadf5bf4324a2579dc60c0d5f20b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:ba0099c87967ad3deca5640c926c7a8f103bc8ff530c6adf33e154781dc746b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283539305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65a68a3c2ad39fd1c5494952c099752a319159620f8655dda24c4c1174f9b0e1`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:07:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 21:08:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:08:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:08:05 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:08:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:08:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:08:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:08:47 GMT
CMD ["bash"]
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201572245620c3000c316fd1492239ba1b53dde9404e8ad4898ad3ad5149d0a`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 177.3 KB (177335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528594ff3960aa89cd0da4c3dceff027b23e8aa79f131d87885c336fb8a89a9`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 1.9 KB (1933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991516221b05d87cc9aa98a4a73f10a169e4a33f47497712fc27858013debe1`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 209.6 KB (209601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c0aa22f0eed42b3091e88dd92fe1f057ba3031c66338b643ff1945078f33fd`  
		Last Modified: Fri, 24 Apr 2020 21:16:11 GMT  
		Size: 58.7 MB (58669093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58ce7d77b31e6816ff071ce4bc528276c2c3013b2ee8b0034bd59b73e41d1ec`  
		Last Modified: Fri, 24 Apr 2020 21:15:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:76c53e4c69a811901801a57d4cf1e50870e36e3c702642be5a8c60cce5a3a650
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236645845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2142ed3ab42e782e6ca0d450abae153237f4cd029b4f2c1279715ab180ef9f2`
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
# Fri, 24 Apr 2020 11:53:46 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 11:53:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:54:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 11:54:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 11:55:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:55:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 11:55:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:55:30 GMT
CMD ["bash"]
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
	-	`sha256:0bad75f33094b614b5bfa5655ddce2210323fb7103d02c9ed57e106baf650cf8`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 177.4 KB (177405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba9633ff2ebf9b850124a9eba586560dfebd225ce62f80388bf42b2a9bc99c`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3306e3aac3a99c454ebf90e8b2cb79752be4ebdfab9a9dd70f49efb235db34c0`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 210.0 KB (209993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d28731e7682f5988588065df3ee6c605004ef8398946cde0ead6f713f1a28`  
		Last Modified: Fri, 24 Apr 2020 12:05:57 GMT  
		Size: 41.0 MB (40961944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8549512425231a158ecb89db00bc97fddf3fab27a4d2e03049fbed925e9435ec`  
		Last Modified: Fri, 24 Apr 2020 12:05:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a8c21cb4efdb75d6f650a101314069e762bd057fb05902927a0fa39166f722eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258362118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8375337e40a0dcf664a1f3991967dfbd082464f3a71de1c351032b99e4a064`
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
# Fri, 24 Apr 2020 15:33:56 GMT
ENV ROS_DISTRO=dashing
# Fri, 24 Apr 2020 15:34:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:34:11 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 15:34:16 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 15:35:30 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:35:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 15:35:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:35:34 GMT
CMD ["bash"]
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
	-	`sha256:168853c0e5c582a7986b59314f3ce5c2ab47f8f2a9d9347f9cca1093e0194b71`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 177.4 KB (177400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1710afaf7ca4719abefac326d77752a6db0f8f43b44924bde460a4b5b179bc39`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85f2813ff6412bbb7db99536c8ec0cc3ae6d08b37c6d3a9c262cac96f44cf7`  
		Last Modified: Fri, 24 Apr 2020 15:45:44 GMT  
		Size: 209.9 KB (209922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a01ecfb5685d76a60d5a301aaf7a4e7b7ef43c49c1be7999f005023a4036`  
		Last Modified: Fri, 24 Apr 2020 15:46:02 GMT  
		Size: 46.2 MB (46179126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0599aa73709e9fd4f80ef366250b76286573192a77ae03cf2729835ddee1d`  
		Last Modified: Fri, 24 Apr 2020 15:45:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent`

```console
$ docker pull ros@sha256:434db188404ebda51f97da352b3a2869cf8636a0e1b8821b59abe1797d566a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent` - linux; amd64

```console
$ docker pull ros@sha256:8e333e3e4fb36443b719fccbd69269430378399dc9b9a092517ebeab74632041
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.3 MB (290333808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155f40a2602a18423705b92c9075790b1968a06076ee7863e243cdfb042535c5`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:09:02 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 21:09:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:09:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:09:11 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:09:47 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:09:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:09:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:09:48 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:10:04 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2b79e32aaee3b1658ae8be4431f31a4b55b07b132269cb547f03242cd7a0b`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 175.6 KB (175559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b76410d2987a1c66329f6c621439e297094a12421f21323234058af9204ff92`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddebdc05dc6896102b59f6f3fb5a3214a504892bc9c5a5cc1cc759f2916e3f8`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 209.6 KB (209593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6db0d488339075fa9ea53cca4378591e553b7140cc9209a3bfb8e1c2c227e2`  
		Last Modified: Fri, 24 Apr 2020 21:16:48 GMT  
		Size: 60.9 MB (60862743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc95fa0e5c4204a361cdd898a1a5011422536260709517dea1673dd09d8041`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c52962224cef30acb287a98905ea27219b4313fccd89cb5b4b6b146d47f1987`  
		Last Modified: Fri, 24 Apr 2020 21:16:54 GMT  
		Size: 4.6 MB (4602672 bytes)  
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

## `ros:eloquent-ros-base`

```console
$ docker pull ros@sha256:434db188404ebda51f97da352b3a2869cf8636a0e1b8821b59abe1797d566a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8e333e3e4fb36443b719fccbd69269430378399dc9b9a092517ebeab74632041
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.3 MB (290333808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155f40a2602a18423705b92c9075790b1968a06076ee7863e243cdfb042535c5`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:09:02 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 21:09:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:09:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:09:11 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:09:47 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:09:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:09:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:09:48 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:10:04 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2b79e32aaee3b1658ae8be4431f31a4b55b07b132269cb547f03242cd7a0b`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 175.6 KB (175559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b76410d2987a1c66329f6c621439e297094a12421f21323234058af9204ff92`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddebdc05dc6896102b59f6f3fb5a3214a504892bc9c5a5cc1cc759f2916e3f8`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 209.6 KB (209593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6db0d488339075fa9ea53cca4378591e553b7140cc9209a3bfb8e1c2c227e2`  
		Last Modified: Fri, 24 Apr 2020 21:16:48 GMT  
		Size: 60.9 MB (60862743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc95fa0e5c4204a361cdd898a1a5011422536260709517dea1673dd09d8041`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c52962224cef30acb287a98905ea27219b4313fccd89cb5b4b6b146d47f1987`  
		Last Modified: Fri, 24 Apr 2020 21:16:54 GMT  
		Size: 4.6 MB (4602672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm variant v7

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

### `ros:eloquent-ros-base` - linux; arm64 variant v8

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

## `ros:eloquent-ros-base-bionic`

```console
$ docker pull ros@sha256:434db188404ebda51f97da352b3a2869cf8636a0e1b8821b59abe1797d566a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:8e333e3e4fb36443b719fccbd69269430378399dc9b9a092517ebeab74632041
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.3 MB (290333808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155f40a2602a18423705b92c9075790b1968a06076ee7863e243cdfb042535c5`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:09:02 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 21:09:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:09:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:09:11 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:09:47 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:09:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:09:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:09:48 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:10:04 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2b79e32aaee3b1658ae8be4431f31a4b55b07b132269cb547f03242cd7a0b`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 175.6 KB (175559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b76410d2987a1c66329f6c621439e297094a12421f21323234058af9204ff92`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddebdc05dc6896102b59f6f3fb5a3214a504892bc9c5a5cc1cc759f2916e3f8`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 209.6 KB (209593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6db0d488339075fa9ea53cca4378591e553b7140cc9209a3bfb8e1c2c227e2`  
		Last Modified: Fri, 24 Apr 2020 21:16:48 GMT  
		Size: 60.9 MB (60862743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc95fa0e5c4204a361cdd898a1a5011422536260709517dea1673dd09d8041`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c52962224cef30acb287a98905ea27219b4313fccd89cb5b4b6b146d47f1987`  
		Last Modified: Fri, 24 Apr 2020 21:16:54 GMT  
		Size: 4.6 MB (4602672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm variant v7

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

### `ros:eloquent-ros-base-bionic` - linux; arm64 variant v8

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

## `ros:eloquent-ros-core`

```console
$ docker pull ros@sha256:595e9775b54b49ca9df7fde4d40446cc9f390e8d3cd77499bee525e8c6e2e199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:3180f972542f55dd216580a5d904f0c79c97cf2e28053dba9fce0bca341b3223
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.7 MB (285731136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c115ec4199cfe4e83b30c2f70f7abf6b5796d45f23f0275cf8cac5ca37af2a47`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:09:02 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 21:09:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:09:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:09:11 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:09:47 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:09:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:09:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:09:48 GMT
CMD ["bash"]
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2b79e32aaee3b1658ae8be4431f31a4b55b07b132269cb547f03242cd7a0b`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 175.6 KB (175559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b76410d2987a1c66329f6c621439e297094a12421f21323234058af9204ff92`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddebdc05dc6896102b59f6f3fb5a3214a504892bc9c5a5cc1cc759f2916e3f8`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 209.6 KB (209593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6db0d488339075fa9ea53cca4378591e553b7140cc9209a3bfb8e1c2c227e2`  
		Last Modified: Fri, 24 Apr 2020 21:16:48 GMT  
		Size: 60.9 MB (60862743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc95fa0e5c4204a361cdd898a1a5011422536260709517dea1673dd09d8041`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:253f7869ffe674e30a21220bfc6ad2e900fdd19a86572fdeca6e788b9416f4d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.4 MB (238411711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005fee40aa7a2803784bfc3fdf05ed40c2cc14f40a623b226dc72461e7539913`
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

### `ros:eloquent-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87ce071670f2c926aac375a5813734717c88628c7b10a1feca278362917e98eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.4 MB (260385195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e470426f06035164465a19d114e93b7800779ea978b1bfa891685877cb2da7`
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

## `ros:eloquent-ros-core-bionic`

```console
$ docker pull ros@sha256:595e9775b54b49ca9df7fde4d40446cc9f390e8d3cd77499bee525e8c6e2e199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:3180f972542f55dd216580a5d904f0c79c97cf2e28053dba9fce0bca341b3223
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.7 MB (285731136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c115ec4199cfe4e83b30c2f70f7abf6b5796d45f23f0275cf8cac5ca37af2a47`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 21:07:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Apr 2020 21:07:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 21:07:55 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 21:09:02 GMT
ENV ROS_DISTRO=eloquent
# Fri, 24 Apr 2020 21:09:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 21:09:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Apr 2020 21:09:11 GMT
RUN pip3 install -U     argcomplete
# Fri, 24 Apr 2020 21:09:47 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:09:48 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Apr 2020 21:09:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 21:09:48 GMT
CMD ["bash"]
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c0ae49a8e18ed2bb693cb4c190d386553e61de7ac2828628b20ec16ea16c6`  
		Last Modified: Fri, 24 Apr 2020 21:16:19 GMT  
		Size: 159.1 MB (159072871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9808ae99c6ff688d2be2dbf4fbee1e02eeb6519ddcd5703949bb01b7de8c93`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ceb42595cdac77bcb3724b2fe30738fe3251bb4aaa53ed795c40188c27c3fe`  
		Last Modified: Fri, 24 Apr 2020 21:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580a16a2772d81a1e6079d8b2555041d5a0759694f192dcfbc3d347aadb76675`  
		Last Modified: Fri, 24 Apr 2020 21:16:02 GMT  
		Size: 37.8 MB (37842961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2b79e32aaee3b1658ae8be4431f31a4b55b07b132269cb547f03242cd7a0b`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 175.6 KB (175559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b76410d2987a1c66329f6c621439e297094a12421f21323234058af9204ff92`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddebdc05dc6896102b59f6f3fb5a3214a504892bc9c5a5cc1cc759f2916e3f8`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 209.6 KB (209593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6db0d488339075fa9ea53cca4378591e553b7140cc9209a3bfb8e1c2c227e2`  
		Last Modified: Fri, 24 Apr 2020 21:16:48 GMT  
		Size: 60.9 MB (60862743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc95fa0e5c4204a361cdd898a1a5011422536260709517dea1673dd09d8041`  
		Last Modified: Fri, 24 Apr 2020 21:16:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:253f7869ffe674e30a21220bfc6ad2e900fdd19a86572fdeca6e788b9416f4d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.4 MB (238411711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005fee40aa7a2803784bfc3fdf05ed40c2cc14f40a623b226dc72461e7539913`
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

### `ros:eloquent-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87ce071670f2c926aac375a5813734717c88628c7b10a1feca278362917e98eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.4 MB (260385195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e470426f06035164465a19d114e93b7800779ea978b1bfa891685877cb2da7`
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

## `ros:kinetic`

```console
$ docker pull ros@sha256:decaa82c78f5787ba83a0c80712dcf04fc55f25431500f47e961a0cf6bcb9418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:4fa62d98dad19374f9e4ad5f7f505669f4e4b026186a67c05b2e3ac91af3004f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.3 MB (385329167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb983727679d36ccabb54873949057a772ebfecbeb2c719e5a313bd5e7ba301b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:022227040356860408a0b0318742da0fe61b05e56ad661eb6b543c2888666bea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336527221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96abb4ad47ce88f35a9926688e4fb39ad008bfde7b2c927ad0658cbced7cce2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f0056b2c74d6f2770d60a914d46cf065bcb0faa0a7ad23376d235d317c0ca46c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.3 MB (350347775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1098c75cb8ea4e5d067727a5000d388d6730a216d7717b11e02a88b008b2e42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:55de0dc7520770765a65fd243757848bf4e57c7a8a1623bc55b1c72714eab95b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:dd3659fefdd4199b7f0d515f2b4bf8bd752b7ec53c1455a9acb3eeb20277c40a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.8 MB (725779572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af2aa0387406a24578a1d6367d34c898b2b0d3396b478e904c4875314c5f272`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:54:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d260503e3b82c736351a8a3aead439505ca09c86fcc5efbb2daf185afbb98`  
		Last Modified: Fri, 24 Apr 2020 21:12:56 GMT  
		Size: 340.5 MB (340450405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:317d5c1b5d012991928bedd4a9398597d42a583b607bb208a13179674f7c8a5c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.1 MB (617056080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebc9e9c17c9a7accc864d43b99537451b26762ef96c870e09304d72890d21a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:39:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddbbde61ec828e11397caa2b530e992da4387f0a12c88e2829105c6206569c8`  
		Last Modified: Fri, 24 Apr 2020 12:01:45 GMT  
		Size: 280.5 MB (280528859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ff872a1c42d591b6b90ac8b49c29b7c6e9b551e0c99e53670191b8038ea92c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.3 MB (641325573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6056370bd573c87e73e47b99230834bd7a21c2a9dbaceae076b642966ab9479`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:16:47 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b11c2a42d033e8345f7b8810beddcabccdb7a04bf52b319f0221ec587d40aee`  
		Last Modified: Fri, 24 Apr 2020 15:42:03 GMT  
		Size: 291.0 MB (290977798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:55de0dc7520770765a65fd243757848bf4e57c7a8a1623bc55b1c72714eab95b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:dd3659fefdd4199b7f0d515f2b4bf8bd752b7ec53c1455a9acb3eeb20277c40a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.8 MB (725779572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af2aa0387406a24578a1d6367d34c898b2b0d3396b478e904c4875314c5f272`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:54:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d260503e3b82c736351a8a3aead439505ca09c86fcc5efbb2daf185afbb98`  
		Last Modified: Fri, 24 Apr 2020 21:12:56 GMT  
		Size: 340.5 MB (340450405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:317d5c1b5d012991928bedd4a9398597d42a583b607bb208a13179674f7c8a5c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.1 MB (617056080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebc9e9c17c9a7accc864d43b99537451b26762ef96c870e09304d72890d21a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:39:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddbbde61ec828e11397caa2b530e992da4387f0a12c88e2829105c6206569c8`  
		Last Modified: Fri, 24 Apr 2020 12:01:45 GMT  
		Size: 280.5 MB (280528859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ff872a1c42d591b6b90ac8b49c29b7c6e9b551e0c99e53670191b8038ea92c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.3 MB (641325573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6056370bd573c87e73e47b99230834bd7a21c2a9dbaceae076b642966ab9479`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:16:47 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b11c2a42d033e8345f7b8810beddcabccdb7a04bf52b319f0221ec587d40aee`  
		Last Modified: Fri, 24 Apr 2020 15:42:03 GMT  
		Size: 291.0 MB (290977798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:a75f22cbe53565989872286fe7c19167169ca6cb7bf68291c2f0b50cc9cac49c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:396d474d9a5c63af304ddc3674db9a506e964c2b089d92dc6ef82178b8f87b2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.1 MB (407093206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b9170bd80ae3e409abe6c9a8e12bfd60480ccab651b0983a1fc99f15eeba26`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:51:07 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bdd9211782b6b0e7e6c56d9d803dd0030b8f159092d9cddd3dd0e7e7c49896`  
		Last Modified: Fri, 24 Apr 2020 21:11:42 GMT  
		Size: 21.8 MB (21764039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:5b203bae2b05e53b129098b793be440d267e20fe64e926c2afcee88e773581d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.6 MB (356567761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7de13885ae38178f9b3750445f8c93cfc2f06f35d2ae6a4361535385c792f58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:36:14 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09399ac033d800caa02630f17b4af27c6b19cc93f041163f957e5015baa28e0e`  
		Last Modified: Fri, 24 Apr 2020 12:00:15 GMT  
		Size: 20.0 MB (20040540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8a3af6308cba8d1eff97b59b619037c6457317536b3a5a1336a1875e34ad04cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371294215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375127b34ecddbcedfb59b3cbdc390ac4c758e7f8754991c3bcb0466dc4d915`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:13:02 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3f8ec5c566ac5bd6472a209d5c9b8d93528b9cfcd6ba74eb56d5d1e78ed1a8`  
		Last Modified: Fri, 24 Apr 2020 15:40:30 GMT  
		Size: 20.9 MB (20946440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:a75f22cbe53565989872286fe7c19167169ca6cb7bf68291c2f0b50cc9cac49c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:396d474d9a5c63af304ddc3674db9a506e964c2b089d92dc6ef82178b8f87b2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.1 MB (407093206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b9170bd80ae3e409abe6c9a8e12bfd60480ccab651b0983a1fc99f15eeba26`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:51:07 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bdd9211782b6b0e7e6c56d9d803dd0030b8f159092d9cddd3dd0e7e7c49896`  
		Last Modified: Fri, 24 Apr 2020 21:11:42 GMT  
		Size: 21.8 MB (21764039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:5b203bae2b05e53b129098b793be440d267e20fe64e926c2afcee88e773581d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.6 MB (356567761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7de13885ae38178f9b3750445f8c93cfc2f06f35d2ae6a4361535385c792f58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:36:14 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09399ac033d800caa02630f17b4af27c6b19cc93f041163f957e5015baa28e0e`  
		Last Modified: Fri, 24 Apr 2020 12:00:15 GMT  
		Size: 20.0 MB (20040540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8a3af6308cba8d1eff97b59b619037c6457317536b3a5a1336a1875e34ad04cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371294215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375127b34ecddbcedfb59b3cbdc390ac4c758e7f8754991c3bcb0466dc4d915`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:13:02 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3f8ec5c566ac5bd6472a209d5c9b8d93528b9cfcd6ba74eb56d5d1e78ed1a8`  
		Last Modified: Fri, 24 Apr 2020 15:40:30 GMT  
		Size: 20.9 MB (20946440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:decaa82c78f5787ba83a0c80712dcf04fc55f25431500f47e961a0cf6bcb9418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:4fa62d98dad19374f9e4ad5f7f505669f4e4b026186a67c05b2e3ac91af3004f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.3 MB (385329167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb983727679d36ccabb54873949057a772ebfecbeb2c719e5a313bd5e7ba301b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:022227040356860408a0b0318742da0fe61b05e56ad661eb6b543c2888666bea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336527221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96abb4ad47ce88f35a9926688e4fb39ad008bfde7b2c927ad0658cbced7cce2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f0056b2c74d6f2770d60a914d46cf065bcb0faa0a7ad23376d235d317c0ca46c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.3 MB (350347775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1098c75cb8ea4e5d067727a5000d388d6730a216d7717b11e02a88b008b2e42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:decaa82c78f5787ba83a0c80712dcf04fc55f25431500f47e961a0cf6bcb9418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:4fa62d98dad19374f9e4ad5f7f505669f4e4b026186a67c05b2e3ac91af3004f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.3 MB (385329167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb983727679d36ccabb54873949057a772ebfecbeb2c719e5a313bd5e7ba301b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 20:50:35 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538f7c842b938e732b13a79765fd2f941c918aee46823f3afc508156b84c63b`  
		Last Modified: Fri, 24 Apr 2020 21:11:33 GMT  
		Size: 85.5 MB (85525614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:022227040356860408a0b0318742da0fe61b05e56ad661eb6b543c2888666bea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336527221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96abb4ad47ce88f35a9926688e4fb39ad008bfde7b2c927ad0658cbced7cce2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:35:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b425b45e58aebd5219e581025c05c0070c611538f457e60f1b814686b8785`  
		Last Modified: Fri, 24 Apr 2020 11:59:53 GMT  
		Size: 76.3 MB (76326391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f0056b2c74d6f2770d60a914d46cf065bcb0faa0a7ad23376d235d317c0ca46c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.3 MB (350347775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1098c75cb8ea4e5d067727a5000d388d6730a216d7717b11e02a88b008b2e42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:12:16 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ece8941d3823b826fd1c431b0c6e3d12360beb4ae9b59411ef07caa7888ce`  
		Last Modified: Fri, 24 Apr 2020 15:40:16 GMT  
		Size: 77.8 MB (77819864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:9c18a26d06592c332ad93f46f9fb90db42ca557596b085767f00d17489aa5ec2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:d1650303967a3ec3289039f7c66237adbe50bee8fe19cc794377923bb157830d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299803553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d665cc6b0a82859d377f77d0d57d2e5e1f18d8f1825059f890945ea0e372944`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:50db698e56119f91d42e86ef14182c4565199cf84d04c33fe55397e2c95275b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260200830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d004bd27a3c1c8c78412e8193fee25297354f13b2966da79affe30e1ff05d17`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e5b950967d66770feb66eb4d67c083756551f0b457218dac5abf6934de2eab78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.5 MB (272527911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0505c253b7a0bf0220b5c35ef4a88d5f04b8525ebc36f3bfac0cd89e24ca9fea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:9c18a26d06592c332ad93f46f9fb90db42ca557596b085767f00d17489aa5ec2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:d1650303967a3ec3289039f7c66237adbe50bee8fe19cc794377923bb157830d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299803553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d665cc6b0a82859d377f77d0d57d2e5e1f18d8f1825059f890945ea0e372944`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:46:34 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:46:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:46:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:47:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:47:18 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 20:47:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:49:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:49:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:49:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:49:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc5fb3503cef1f5ff32b818035c1219faef0f8537b7ae31801418cc2c2f2a2`  
		Last Modified: Fri, 24 Apr 2020 21:10:22 GMT  
		Size: 6.9 MB (6936473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e21ec5cdfbae18990f30735b7b9828a18edcb8c830fd254e12adcda8f33b9`  
		Last Modified: Fri, 24 Apr 2020 21:10:21 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d26f628f675b503ffd3214c6f7f6bc9998ea6e58dcf5a6383668fb42ca3d12`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7737f190310e82ece9e301a28dd3e5a41b4621d663a4b96ea3ace7b964e7656`  
		Last Modified: Fri, 24 Apr 2020 21:10:34 GMT  
		Size: 54.8 MB (54790036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec575ad79465df1013d0dbac2313c5ed95a9ee139ecf0aab9ff390e9fca20d4`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 253.6 KB (253595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84296616d772863d7fd73fd41703bd301e0c4ce55cb2b9a6fe3368d61bd582`  
		Last Modified: Fri, 24 Apr 2020 21:11:04 GMT  
		Size: 193.6 MB (193561245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41803963b06568632321145bf5de5acf1b2ae55a102201855d136b24cc623d`  
		Last Modified: Fri, 24 Apr 2020 21:10:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:50db698e56119f91d42e86ef14182c4565199cf84d04c33fe55397e2c95275b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260200830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d004bd27a3c1c8c78412e8193fee25297354f13b2966da79affe30e1ff05d17`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:30:05 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:30:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:30:10 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:31:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:31:21 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:31:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:31:23 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 11:31:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:33:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:33:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:33:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:33:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6b68f3d41b9f69a317613dc09fbb7bbd90e74a633d3d4cd82883740dc61f9`  
		Last Modified: Fri, 24 Apr 2020 11:58:34 GMT  
		Size: 5.7 MB (5700698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b2a2b38a66d74db9685123dbd74d305072081e3be996b1bbc27dab42efc53`  
		Last Modified: Fri, 24 Apr 2020 11:58:33 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5984390cba2b35cadbc00adb04a91fc17112a1743ff6c761502f564457931e81`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1480cbc19af5716cdd5cfb5933c0eedecae676e73c66da7a017cb9c911b93425`  
		Last Modified: Fri, 24 Apr 2020 11:58:49 GMT  
		Size: 50.4 MB (50352264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb115936c3a9df41806d09e9d15c9a2ba0ad819ad677ea1a99a79c617721e472`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 253.6 KB (253596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712e7c8e4bd80b089ebd8bf85b34aae8d3ee7701eeab9d09dc9afb172a46053`  
		Last Modified: Fri, 24 Apr 2020 11:59:21 GMT  
		Size: 165.0 MB (164957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f481d9aac9ef6966403b693b4a07e5803633042543e7c49be213fe5ed7be7af`  
		Last Modified: Fri, 24 Apr 2020 11:58:31 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e5b950967d66770feb66eb4d67c083756551f0b457218dac5abf6934de2eab78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.5 MB (272527911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0505c253b7a0bf0220b5c35ef4a88d5f04b8525ebc36f3bfac0cd89e24ca9fea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:07:24 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:07:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:08:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:08:35 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:08:36 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Apr 2020 15:08:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:10:46 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:10:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:10:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:10:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c90921649b9f3cbb166f1e7855183c9279e66255ecccdacd8d50ab227b51d`  
		Last Modified: Fri, 24 Apr 2020 15:38:58 GMT  
		Size: 6.0 MB (5958923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746fe22f751624a02dac2053e33f6f9ff3c7d7b8b49c425e95ca0c7070f5bb7e`  
		Last Modified: Fri, 24 Apr 2020 15:38:57 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c987dca6dd6b9fe0c80f563b4875bff8dcc141b5f34cfb4e1eb8c01a0b6d0d`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18bb8b026ed4b9b7a7353ad77f25040546e8fef3518489ad6e6142c506086c`  
		Last Modified: Fri, 24 Apr 2020 15:39:13 GMT  
		Size: 52.1 MB (52080831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaa0f6e5606c1bba121e6d0dbe69a81288185397dc350cda105e68362d1ec5e`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 253.6 KB (253640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d24e768d1998989be9ded331fa29a8c50e23d0fabff7bc8c69452f42bc1a`  
		Last Modified: Fri, 24 Apr 2020 15:39:48 GMT  
		Size: 174.3 MB (174250705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fc9d55b1c4856d7d6f7313254ada25174fc64b5d913da70b72cfd07d550e0`  
		Last Modified: Fri, 24 Apr 2020 15:38:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:bf9a8210833f8544e79d1d356c1b0c7514ab72f88ada968c952d98c2226028af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:b4dfc109dcc86fe8832cd9080c654ceca9105f89adeb1c3e53eed3ad6e8a5680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436672443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9891a039b3f33a89fcdf7f90850020b958e94fb01c43d240b5518e635c900202`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm variant v7

```console
$ docker pull ros@sha256:ef50d4f351a92110bfddb63b5350bc59808597f87219daba9ec3e3ffebbc175b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385350213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5eeea6428a9735c970227fb486b0fa20bcfde99b4cfb56cc015612c7278d4c`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:643df2fec4dbfa918429d893844525478c8296903002493baaa671327a2a285d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411700540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673fc41f5c1c9decafd16ec0131723228a4e306ff56cbaf7bbfef6c29f2cd05c`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:bf9a8210833f8544e79d1d356c1b0c7514ab72f88ada968c952d98c2226028af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:b4dfc109dcc86fe8832cd9080c654ceca9105f89adeb1c3e53eed3ad6e8a5680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436672443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9891a039b3f33a89fcdf7f90850020b958e94fb01c43d240b5518e635c900202`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ef50d4f351a92110bfddb63b5350bc59808597f87219daba9ec3e3ffebbc175b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385350213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5eeea6428a9735c970227fb486b0fa20bcfde99b4cfb56cc015612c7278d4c`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:643df2fec4dbfa918429d893844525478c8296903002493baaa671327a2a285d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411700540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673fc41f5c1c9decafd16ec0131723228a4e306ff56cbaf7bbfef6c29f2cd05c`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:ac084c820f933339609883a5e7cc7b75df8298faa45948c0fdfd03b1e993ba4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:752e513dd3989e910d4b37519b8ef0abf9271d8ae5838247b894beef861a50a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 MB (786975875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f861f63ecb6a2c134eaf2fdcac8a074a961f2c023134d4487c39d1def06f70d5`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:06:15 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197cfc685ae274f7e7558b7483cd3c20ec43ab1b23cce0dd879fcefcd24138bb`  
		Last Modified: Fri, 24 Apr 2020 21:15:45 GMT  
		Size: 350.3 MB (350303432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:f530f1e6f199e452afd897b866292c46e902bce5ab057f8a2dade785d7c8ab8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **685.6 MB (685606488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6a48d42941d8b28596d17b6fb2888486209375bf524dbb557aacc0e93eb4e6`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:51:00 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb34278c6d425e9ed667bc3a179e2c014716cff8e45b01be8fe88209832734`  
		Last Modified: Fri, 24 Apr 2020 12:05:31 GMT  
		Size: 300.3 MB (300256275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d74f0444a442ee789f8848cf96f55716621d26289f09d78a29ea9083000d912f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **744.6 MB (744645250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65dc138b2649dfd4b4e64ae2fd96433af700c407995d7af50874c7e45bd3b007`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:30:47 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a03a2d0c0e2249cd00bfc34002c9986b7268549bbb3de1d1ab5441b6cd0e57`  
		Last Modified: Fri, 24 Apr 2020 15:45:36 GMT  
		Size: 332.9 MB (332944710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:ac084c820f933339609883a5e7cc7b75df8298faa45948c0fdfd03b1e993ba4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:752e513dd3989e910d4b37519b8ef0abf9271d8ae5838247b894beef861a50a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 MB (786975875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f861f63ecb6a2c134eaf2fdcac8a074a961f2c023134d4487c39d1def06f70d5`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:06:15 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197cfc685ae274f7e7558b7483cd3c20ec43ab1b23cce0dd879fcefcd24138bb`  
		Last Modified: Fri, 24 Apr 2020 21:15:45 GMT  
		Size: 350.3 MB (350303432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f530f1e6f199e452afd897b866292c46e902bce5ab057f8a2dade785d7c8ab8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **685.6 MB (685606488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6a48d42941d8b28596d17b6fb2888486209375bf524dbb557aacc0e93eb4e6`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:51:00 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb34278c6d425e9ed667bc3a179e2c014716cff8e45b01be8fe88209832734`  
		Last Modified: Fri, 24 Apr 2020 12:05:31 GMT  
		Size: 300.3 MB (300256275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d74f0444a442ee789f8848cf96f55716621d26289f09d78a29ea9083000d912f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **744.6 MB (744645250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65dc138b2649dfd4b4e64ae2fd96433af700c407995d7af50874c7e45bd3b007`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:30:47 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a03a2d0c0e2249cd00bfc34002c9986b7268549bbb3de1d1ab5441b6cd0e57`  
		Last Modified: Fri, 24 Apr 2020 15:45:36 GMT  
		Size: 332.9 MB (332944710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:9fce569f7b3f7e962d913b67c379b534097c4bfb8612f6afa6933415c66339e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:351c5bd25617d3d594b9234a17c06233ad9f902774bdd0f79e3e6ef30ee124a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **882.0 MB (881985049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed8aa44dd3bcc791e368ad944014159ff1b1205f461aac0870d2b738a0d8963`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Sat, 16 May 2020 03:59:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 03:59:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 May 2020 03:59:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 May 2020 04:00:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:00:07 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 04:00:07 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 May 2020 04:00:08 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 May 2020 04:00:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 May 2020 04:01:52 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:01:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 May 2020 04:01:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 May 2020 04:01:54 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:02:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:05:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fda4a46c1d10f88aabb05da22ec1b0b29e36528fa63d6ad5d315eef32b04d0`  
		Last Modified: Sat, 16 May 2020 04:06:33 GMT  
		Size: 10.5 MB (10476838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74529292be06ac11f652a0185d3b8a8e7c8e6318f78145c9fc6a1f62ab665d83`  
		Last Modified: Sat, 16 May 2020 04:06:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9068d1ad5bb66c7ce4974550fa3d9bd1a50ddd06b3aff537cf8ac34edf7dbc7b`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a7091997ccf0c3afb96ac38925f448e86129e61725cd384d216b8db2da380`  
		Last Modified: Sat, 16 May 2020 04:06:47 GMT  
		Size: 64.8 MB (64797298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3728aa494cb44476d46affef19ab460b7bc376333944a5db9eee751da17d8981`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 247.7 KB (247672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892457fe31ca1f052dc113ae893fb097c7f869363701bc2762a648f9547db9e`  
		Last Modified: Sat, 16 May 2020 04:07:20 GMT  
		Size: 276.2 MB (276209403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39976de06deee43924e049833042e4781f041b7fbf3f42687e6e26ae32a2e98d`  
		Last Modified: Sat, 16 May 2020 04:06:29 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec696c745f89d6b37ff9dec480e2f40cf8471a1cbcc62e5cf79f607183ddd46`  
		Last Modified: Sat, 16 May 2020 04:07:44 GMT  
		Size: 108.5 MB (108477140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70006463acdf2d2672fb9ea4116349cad98ef8264e4bc345c24d8960c014765`  
		Last Modified: Sat, 16 May 2020 04:09:06 GMT  
		Size: 376.4 MB (376399668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:83b3dd0ff436f631c1bcbf9f455e0ad69ff8e1a50a94f02560a7d7fb09f8c634
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **799.8 MB (799772563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d3ebf8f45dd3d84e55b9dd124ed6c53c875a7a77cc3d17885b6bef2b7a8cf7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:19:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:19:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Apr 2020 10:19:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Apr 2020 10:20:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:21:02 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 10:21:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Apr 2020 10:21:04 GMT
ENV ROS_DISTRO=melodic
# Thu, 23 Apr 2020 10:21:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Apr 2020 10:24:02 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:24:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 23 Apr 2020 10:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Apr 2020 10:24:16 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:32:06 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b84e9b12c5036e24d270012ffc332ba283c66c65bb1a11c9c36b62ac52c316`  
		Last Modified: Thu, 23 Apr 2020 10:33:34 GMT  
		Size: 9.8 MB (9774901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863092d8428511c061a2c0340a7ec4d93abf5f123245890332e777c71423f808`  
		Last Modified: Thu, 23 Apr 2020 10:33:30 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b36b14c03269a863c72850458f82fa87b8d312d31a723483b3f5702fdc05a2`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2835519f2d237d39236d2dce0f921f1a6dfd9c0631be6c87023f67600d84dcb`  
		Last Modified: Thu, 23 Apr 2020 10:33:48 GMT  
		Size: 62.1 MB (62097551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f60228a5fb4c85cc691071f60a0fc0154ee013df14567edd599f828c3b6ad`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 243.1 KB (243119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00549af9a42e3dd1e9bc8593968eee697343c02e19600216d07d73c9874cc`  
		Last Modified: Thu, 23 Apr 2020 10:34:38 GMT  
		Size: 230.4 MB (230401327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619c48071b4dbff1dd36122924749c4e683b84b45a23f252dd209bc3f04d4ada`  
		Last Modified: Thu, 23 Apr 2020 10:33:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7aa7bc01ef2228d72d31cf584f125210e89f0a44ebdc2eedbcc4226fd48c2f`  
		Last Modified: Thu, 23 Apr 2020 10:35:13 GMT  
		Size: 103.0 MB (102958711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180ea1c2048cd03d55e879ef2fb234a75b825de33aa4241418ca074c776cc072`  
		Last Modified: Thu, 23 Apr 2020 10:37:16 GMT  
		Size: 351.1 MB (351136113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:9a21e7b6932df7441b8a1c537ef94041fc1ba6bc79f14c8c434b7a2b1bf1eaf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:83c85d5c50f3462ed136f5752aad935f9bfb99a1d6a1078673a5465bc4289352
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449090119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8eacc10a69686fa2443325ce41ecae562c2b99c3a8f3b5a3553033da7389fa`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:00:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ca25dd0fd452bf5bf43d4828d39b869e21da20c5395923342dd5952b61fce`  
		Last Modified: Fri, 24 Apr 2020 21:14:30 GMT  
		Size: 12.4 MB (12417676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:59af0378e0da7efc93e669ed4c8eb1641be780e50c2e4d6daec4a15b9ec13471
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.8 MB (396833017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a7c1eff0a43706aff973685ca9fedee4ea07f819c8439f19683a0eaca33978`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:47:00 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3b773f8eb33730d1d2cd16aaeff3614829db79eaad144103ad868f52801197`  
		Last Modified: Fri, 24 Apr 2020 12:03:52 GMT  
		Size: 11.5 MB (11482804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:67c053f098ab333576b40b7ab16322c504f9f9da1d162b6fe8037765a58a151f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.8 MB (423780761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1fae7c19aef4f9c8db9b8891b882f2d5a18d8a8d8739b167ae63e0937489c0`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:25:48 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9674ce76a71aad485660cef98494d1a329b1028a667c95d4b9b2cdf4a1ca12`  
		Last Modified: Fri, 24 Apr 2020 15:43:53 GMT  
		Size: 12.1 MB (12080221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:9a21e7b6932df7441b8a1c537ef94041fc1ba6bc79f14c8c434b7a2b1bf1eaf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:83c85d5c50f3462ed136f5752aad935f9bfb99a1d6a1078673a5465bc4289352
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449090119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8eacc10a69686fa2443325ce41ecae562c2b99c3a8f3b5a3553033da7389fa`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:00:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ca25dd0fd452bf5bf43d4828d39b869e21da20c5395923342dd5952b61fce`  
		Last Modified: Fri, 24 Apr 2020 21:14:30 GMT  
		Size: 12.4 MB (12417676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:59af0378e0da7efc93e669ed4c8eb1641be780e50c2e4d6daec4a15b9ec13471
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.8 MB (396833017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a7c1eff0a43706aff973685ca9fedee4ea07f819c8439f19683a0eaca33978`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:47:00 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3b773f8eb33730d1d2cd16aaeff3614829db79eaad144103ad868f52801197`  
		Last Modified: Fri, 24 Apr 2020 12:03:52 GMT  
		Size: 11.5 MB (11482804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:67c053f098ab333576b40b7ab16322c504f9f9da1d162b6fe8037765a58a151f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.8 MB (423780761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1fae7c19aef4f9c8db9b8891b882f2d5a18d8a8d8739b167ae63e0937489c0`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:25:48 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9674ce76a71aad485660cef98494d1a329b1028a667c95d4b9b2cdf4a1ca12`  
		Last Modified: Fri, 24 Apr 2020 15:43:53 GMT  
		Size: 12.1 MB (12080221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:bf5c952c1ff10d129343a840593f5e6128e721fc54cacaea456f6bae6f84de19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:b1704c8ca03d4e703213ace2713c3297f453c5ea1febb468ed971cf801837406
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.1 MB (522113757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b16dd60fbb6e92942d9d16dd706b4ea44ced173b33ed04bf9b8aac10d4d68be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Sat, 16 May 2020 03:59:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 03:59:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 May 2020 03:59:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 May 2020 04:00:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:00:07 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 04:00:07 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 May 2020 04:00:08 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 May 2020 04:00:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 May 2020 04:01:52 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:01:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 May 2020 04:01:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 May 2020 04:01:54 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:02:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:03:23 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fda4a46c1d10f88aabb05da22ec1b0b29e36528fa63d6ad5d315eef32b04d0`  
		Last Modified: Sat, 16 May 2020 04:06:33 GMT  
		Size: 10.5 MB (10476838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74529292be06ac11f652a0185d3b8a8e7c8e6318f78145c9fc6a1f62ab665d83`  
		Last Modified: Sat, 16 May 2020 04:06:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9068d1ad5bb66c7ce4974550fa3d9bd1a50ddd06b3aff537cf8ac34edf7dbc7b`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a7091997ccf0c3afb96ac38925f448e86129e61725cd384d216b8db2da380`  
		Last Modified: Sat, 16 May 2020 04:06:47 GMT  
		Size: 64.8 MB (64797298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3728aa494cb44476d46affef19ab460b7bc376333944a5db9eee751da17d8981`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 247.7 KB (247672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892457fe31ca1f052dc113ae893fb097c7f869363701bc2762a648f9547db9e`  
		Last Modified: Sat, 16 May 2020 04:07:20 GMT  
		Size: 276.2 MB (276209403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39976de06deee43924e049833042e4781f041b7fbf3f42687e6e26ae32a2e98d`  
		Last Modified: Sat, 16 May 2020 04:06:29 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec696c745f89d6b37ff9dec480e2f40cf8471a1cbcc62e5cf79f607183ddd46`  
		Last Modified: Sat, 16 May 2020 04:07:44 GMT  
		Size: 108.5 MB (108477140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994586a749a4364a66789c73d9fb05ab961f42f5daacf5f16180ecc7a756740`  
		Last Modified: Sat, 16 May 2020 04:07:50 GMT  
		Size: 16.5 MB (16528376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5a6b72b5bfa25adf48728818246b7e739f8fd331df40670cbcb5f71c869e362b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **464.7 MB (464708978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8abcb5f2e19ee8a6b9a1829f3e4394721baf58a6545c8b823e2da6495babbfc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:19:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:19:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Apr 2020 10:19:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Apr 2020 10:20:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:21:02 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 10:21:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Apr 2020 10:21:04 GMT
ENV ROS_DISTRO=melodic
# Thu, 23 Apr 2020 10:21:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Apr 2020 10:24:02 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:24:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 23 Apr 2020 10:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Apr 2020 10:24:16 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:26:37 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b84e9b12c5036e24d270012ffc332ba283c66c65bb1a11c9c36b62ac52c316`  
		Last Modified: Thu, 23 Apr 2020 10:33:34 GMT  
		Size: 9.8 MB (9774901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863092d8428511c061a2c0340a7ec4d93abf5f123245890332e777c71423f808`  
		Last Modified: Thu, 23 Apr 2020 10:33:30 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b36b14c03269a863c72850458f82fa87b8d312d31a723483b3f5702fdc05a2`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2835519f2d237d39236d2dce0f921f1a6dfd9c0631be6c87023f67600d84dcb`  
		Last Modified: Thu, 23 Apr 2020 10:33:48 GMT  
		Size: 62.1 MB (62097551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f60228a5fb4c85cc691071f60a0fc0154ee013df14567edd599f828c3b6ad`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 243.1 KB (243119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00549af9a42e3dd1e9bc8593968eee697343c02e19600216d07d73c9874cc`  
		Last Modified: Thu, 23 Apr 2020 10:34:38 GMT  
		Size: 230.4 MB (230401327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619c48071b4dbff1dd36122924749c4e683b84b45a23f252dd209bc3f04d4ada`  
		Last Modified: Thu, 23 Apr 2020 10:33:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7aa7bc01ef2228d72d31cf584f125210e89f0a44ebdc2eedbcc4226fd48c2f`  
		Last Modified: Thu, 23 Apr 2020 10:35:13 GMT  
		Size: 103.0 MB (102958711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38737e22deccc64504d87fb8230cf1d7621e11c7ccf121c2e7dcc3ccff3e0aed`  
		Last Modified: Thu, 23 Apr 2020 10:35:25 GMT  
		Size: 16.1 MB (16072528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:bf9a8210833f8544e79d1d356c1b0c7514ab72f88ada968c952d98c2226028af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b4dfc109dcc86fe8832cd9080c654ceca9105f89adeb1c3e53eed3ad6e8a5680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436672443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9891a039b3f33a89fcdf7f90850020b958e94fb01c43d240b5518e635c900202`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:ef50d4f351a92110bfddb63b5350bc59808597f87219daba9ec3e3ffebbc175b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385350213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5eeea6428a9735c970227fb486b0fa20bcfde99b4cfb56cc015612c7278d4c`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:643df2fec4dbfa918429d893844525478c8296903002493baaa671327a2a285d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411700540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673fc41f5c1c9decafd16ec0131723228a4e306ff56cbaf7bbfef6c29f2cd05c`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:bf9a8210833f8544e79d1d356c1b0c7514ab72f88ada968c952d98c2226028af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b4dfc109dcc86fe8832cd9080c654ceca9105f89adeb1c3e53eed3ad6e8a5680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436672443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9891a039b3f33a89fcdf7f90850020b958e94fb01c43d240b5518e635c900202`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 21:00:20 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa25649a1657b66aa7ec13605a16f9ef12593874b26892497981d3a07db719`  
		Last Modified: Fri, 24 Apr 2020 21:14:20 GMT  
		Size: 72.9 MB (72921952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ef50d4f351a92110bfddb63b5350bc59808597f87219daba9ec3e3ffebbc175b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385350213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5eeea6428a9735c970227fb486b0fa20bcfde99b4cfb56cc015612c7278d4c`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 11:46:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca2cf40b081d642195f678626ed8e907a246e5b56d05879a8a33c06193043d`  
		Last Modified: Fri, 24 Apr 2020 12:03:34 GMT  
		Size: 62.9 MB (62881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:643df2fec4dbfa918429d893844525478c8296903002493baaa671327a2a285d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411700540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673fc41f5c1c9decafd16ec0131723228a4e306ff56cbaf7bbfef6c29f2cd05c`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 15:24:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b3f665c2e407aa4986de22c66c0d4d85633e4d15a7a3b5471c33bacacf6353`  
		Last Modified: Fri, 24 Apr 2020 15:43:42 GMT  
		Size: 65.6 MB (65556338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:6f218a96f906d55c67d8c8a0112c1b62d000ca22d5e875ed75c98449300d77f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:b88e0fcc172ad6cb6567486c5cb3ac2a69ecf4ee492a073703412f106b0a27e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **505.6 MB (505585381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232a00554a24f65a0da68531b75e050f3268ce08f965ae1a0ba4e694b91c8df3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Sat, 16 May 2020 03:59:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 03:59:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 May 2020 03:59:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 May 2020 04:00:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:00:07 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 04:00:07 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 May 2020 04:00:08 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 May 2020 04:00:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 May 2020 04:01:52 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:01:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 May 2020 04:01:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 May 2020 04:01:54 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:02:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fda4a46c1d10f88aabb05da22ec1b0b29e36528fa63d6ad5d315eef32b04d0`  
		Last Modified: Sat, 16 May 2020 04:06:33 GMT  
		Size: 10.5 MB (10476838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74529292be06ac11f652a0185d3b8a8e7c8e6318f78145c9fc6a1f62ab665d83`  
		Last Modified: Sat, 16 May 2020 04:06:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9068d1ad5bb66c7ce4974550fa3d9bd1a50ddd06b3aff537cf8ac34edf7dbc7b`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a7091997ccf0c3afb96ac38925f448e86129e61725cd384d216b8db2da380`  
		Last Modified: Sat, 16 May 2020 04:06:47 GMT  
		Size: 64.8 MB (64797298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3728aa494cb44476d46affef19ab460b7bc376333944a5db9eee751da17d8981`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 247.7 KB (247672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892457fe31ca1f052dc113ae893fb097c7f869363701bc2762a648f9547db9e`  
		Last Modified: Sat, 16 May 2020 04:07:20 GMT  
		Size: 276.2 MB (276209403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39976de06deee43924e049833042e4781f041b7fbf3f42687e6e26ae32a2e98d`  
		Last Modified: Sat, 16 May 2020 04:06:29 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec696c745f89d6b37ff9dec480e2f40cf8471a1cbcc62e5cf79f607183ddd46`  
		Last Modified: Sat, 16 May 2020 04:07:44 GMT  
		Size: 108.5 MB (108477140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:72933564cc48bf57b54e2816702e40937b490d4f71ff3e64beb2d92252765470
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448636450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8254326c4a8f06c3e1541e8619b593fc51e99e32baf7fbe25b584cc011edee5d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:19:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:19:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Apr 2020 10:19:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Apr 2020 10:20:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:21:02 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 10:21:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Apr 2020 10:21:04 GMT
ENV ROS_DISTRO=melodic
# Thu, 23 Apr 2020 10:21:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Apr 2020 10:24:02 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:24:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 23 Apr 2020 10:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Apr 2020 10:24:16 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b84e9b12c5036e24d270012ffc332ba283c66c65bb1a11c9c36b62ac52c316`  
		Last Modified: Thu, 23 Apr 2020 10:33:34 GMT  
		Size: 9.8 MB (9774901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863092d8428511c061a2c0340a7ec4d93abf5f123245890332e777c71423f808`  
		Last Modified: Thu, 23 Apr 2020 10:33:30 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b36b14c03269a863c72850458f82fa87b8d312d31a723483b3f5702fdc05a2`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2835519f2d237d39236d2dce0f921f1a6dfd9c0631be6c87023f67600d84dcb`  
		Last Modified: Thu, 23 Apr 2020 10:33:48 GMT  
		Size: 62.1 MB (62097551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f60228a5fb4c85cc691071f60a0fc0154ee013df14567edd599f828c3b6ad`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 243.1 KB (243119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00549af9a42e3dd1e9bc8593968eee697343c02e19600216d07d73c9874cc`  
		Last Modified: Thu, 23 Apr 2020 10:34:38 GMT  
		Size: 230.4 MB (230401327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619c48071b4dbff1dd36122924749c4e683b84b45a23f252dd209bc3f04d4ada`  
		Last Modified: Thu, 23 Apr 2020 10:33:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7aa7bc01ef2228d72d31cf584f125210e89f0a44ebdc2eedbcc4226fd48c2f`  
		Last Modified: Thu, 23 Apr 2020 10:35:13 GMT  
		Size: 103.0 MB (102958711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:9663961790cc7345e54972dfc165cd5fcab52898d6c28d550b35554c35f4186e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ef12771459e452081c07ace95b404f0cf2ef60364e7f0f56faedf2c66d1bcde0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363750491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4308b32c0717bf7c78db0c8cc28971610d0265ec89bf26742c7068629847b1`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:511f45681c68e1e2fd41736d647d862bfc3e5d428955b14348a001eccb54f660
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322468898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cf5d6c1920c86752a24bc223709ec79224917793c942a2a8590d51cb9996d18`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7dcc11e69815fb8962da4396f7ffd77c1dbfc2e6352e7823ba0d3cc238e765ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346144202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaa405de44742ab620c15a6574c1948d06cdd68f1c28a4319113759feb335a0`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:9663961790cc7345e54972dfc165cd5fcab52898d6c28d550b35554c35f4186e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:ef12771459e452081c07ace95b404f0cf2ef60364e7f0f56faedf2c66d1bcde0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363750491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4308b32c0717bf7c78db0c8cc28971610d0265ec89bf26742c7068629847b1`
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
# Fri, 24 Apr 2020 19:46:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:18 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:55:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 20:55:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 20:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 20:56:12 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 20:56:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 20:59:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 20:59:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 20:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 20:59:03 GMT
CMD ["bash"]
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
	-	`sha256:04b393b40dc2efdd5d090642ca477ff4b122fd0da47e0e91cd6c502b7b02de9b`  
		Last Modified: Fri, 24 Apr 2020 20:01:27 GMT  
		Size: 837.5 KB (837497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2b2696e602239579df55b7654cf1f34a33d51795018e963390b817867b84a2`  
		Last Modified: Fri, 24 Apr 2020 21:13:03 GMT  
		Size: 6.8 MB (6779974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22538d7f14dd61f7a7b637513b446b0b52c79083e37a69b98de7de1890d531cd`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2373a951182148130a06e5c1b822a99d4f33b108f224259d7e3a040940c480a0`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b2b078aacce4ad025783c67fd4de35777f4a4fe25872c16d61298e9b9be65c`  
		Last Modified: Fri, 24 Apr 2020 21:13:15 GMT  
		Size: 55.1 MB (55084765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a236411e54d2c90604cc2c4a4e8c2e9a758af4a1a5b5bedfde1687554ee519`  
		Last Modified: Fri, 24 Apr 2020 21:13:00 GMT  
		Size: 243.1 KB (243051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549f3fda09972e87bf554e3172327974bb5f88216cc3372c0931474f9096d1d`  
		Last Modified: Fri, 24 Apr 2020 21:13:58 GMT  
		Size: 274.1 MB (274077195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25914edf367705030fa9758159c357a8e930fa3ba2154fec29888a62a7e5aa`  
		Last Modified: Fri, 24 Apr 2020 21:13:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:511f45681c68e1e2fd41736d647d862bfc3e5d428955b14348a001eccb54f660
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322468898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cf5d6c1920c86752a24bc223709ec79224917793c942a2a8590d51cb9996d18`
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
# Fri, 24 Apr 2020 11:40:52 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:40:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 11:40:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 11:41:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 11:42:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 11:42:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 11:42:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 11:44:49 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:45:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 11:45:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 11:45:02 GMT
CMD ["bash"]
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
	-	`sha256:524268b33129daf643b650e73f128ba53f623b2a24cac42409a6463a41a1cfe7`  
		Last Modified: Fri, 24 Apr 2020 12:02:00 GMT  
		Size: 5.6 MB (5631553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9647b66cca56061029bc67ebc835e2a1becf32c54ea3a9db21eecacc56693e`  
		Last Modified: Fri, 24 Apr 2020 12:01:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c7e7eddbf6a445cb9bb55b927c9e37b9c5d71471f14b2fc79483299f412629`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9d36e31285a2f447213f9c2e5bb71005ebcfeb52784ee946c9836715b2561`  
		Last Modified: Fri, 24 Apr 2020 12:02:13 GMT  
		Size: 50.1 MB (50117141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4e30c4084f438f74a3cdd8979a10fdbe5177a9042c08c72e21114bdb8617d6`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 243.1 KB (243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ded763e2c02786f89b0516722042e8f8c8f8b5388e3350f1637ab38a99ca0e`  
		Last Modified: Fri, 24 Apr 2020 12:03:00 GMT  
		Size: 243.3 MB (243324058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce4eaadd525c48290723f9b302671b945b40981b1b35951f73049f46e3f8302`  
		Last Modified: Fri, 24 Apr 2020 12:01:56 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7dcc11e69815fb8962da4396f7ffd77c1dbfc2e6352e7823ba0d3cc238e765ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346144202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaa405de44742ab620c15a6574c1948d06cdd68f1c28a4319113759feb335a0`
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
# Fri, 24 Apr 2020 15:18:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:18:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Apr 2020 15:18:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Apr 2020 15:19:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 15:19:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Apr 2020 15:19:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 24 Apr 2020 15:19:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Apr 2020 15:23:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:23:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Apr 2020 15:23:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Apr 2020 15:23:35 GMT
CMD ["bash"]
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
	-	`sha256:f8a3dc1850d0b63d684d5925a20ac922d37e39d7f87268010101e07caa0c574b`  
		Last Modified: Fri, 24 Apr 2020 15:42:13 GMT  
		Size: 6.1 MB (6097195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc4248ccf3d851679ffbdd9a0d91de9a960bed8eea46f4d302956e5bb556d17`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376cec84b0dc49127c5dafe67d628c2650a33432182ce4058cb5b46ebd1c2812`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dbddfce4012801c50c7775bdfbe4fcae860aa9bfa35d6d0cb11b2ae14c9158`  
		Last Modified: Fri, 24 Apr 2020 15:42:27 GMT  
		Size: 52.9 MB (52934533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d11c7024fa754e5292634ed00853ed0f16fee35c4f3894cccef0ac9cabfce`  
		Last Modified: Fri, 24 Apr 2020 15:42:10 GMT  
		Size: 243.1 KB (243122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa988f8797da56c41a247dcac44beadbbb16c5ae882548b15a777caab4c4bb`  
		Last Modified: Fri, 24 Apr 2020 15:43:17 GMT  
		Size: 262.3 MB (262272972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b60096075a702d8f90b408e520af84886d1abb831101de165a9bd4eaffcfd`  
		Last Modified: Fri, 24 Apr 2020 15:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:4c9cde0c799c558dbc88aaed2065869e7a66d99bf27d4b8053614cc345f51484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:a9fbf0fdca142715dc3cb1a3df2e45a2e85b578f1845535d1396f2d81fbcf2e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.1 MB (397108241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4a8a25cba7ea79f653285609755146d0fac53cd1e2dcbd6ec5686a6eff5059`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Sat, 16 May 2020 03:59:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 03:59:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 May 2020 03:59:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 May 2020 04:00:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:00:07 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 04:00:07 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 May 2020 04:00:08 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 May 2020 04:00:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 May 2020 04:01:52 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:01:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 May 2020 04:01:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 May 2020 04:01:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fda4a46c1d10f88aabb05da22ec1b0b29e36528fa63d6ad5d315eef32b04d0`  
		Last Modified: Sat, 16 May 2020 04:06:33 GMT  
		Size: 10.5 MB (10476838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74529292be06ac11f652a0185d3b8a8e7c8e6318f78145c9fc6a1f62ab665d83`  
		Last Modified: Sat, 16 May 2020 04:06:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9068d1ad5bb66c7ce4974550fa3d9bd1a50ddd06b3aff537cf8ac34edf7dbc7b`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a7091997ccf0c3afb96ac38925f448e86129e61725cd384d216b8db2da380`  
		Last Modified: Sat, 16 May 2020 04:06:47 GMT  
		Size: 64.8 MB (64797298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3728aa494cb44476d46affef19ab460b7bc376333944a5db9eee751da17d8981`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 247.7 KB (247672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892457fe31ca1f052dc113ae893fb097c7f869363701bc2762a648f9547db9e`  
		Last Modified: Sat, 16 May 2020 04:07:20 GMT  
		Size: 276.2 MB (276209403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39976de06deee43924e049833042e4781f041b7fbf3f42687e6e26ae32a2e98d`  
		Last Modified: Sat, 16 May 2020 04:06:29 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0bc5b0df570463816044360cfc1f671e112c42d3969feeae8540df525d36a8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.7 MB (345677739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c1664b138614872e61e929b18da0af16adc268966a4b28d35df6270da09680`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:19:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:19:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Apr 2020 10:19:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Apr 2020 10:20:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:21:02 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 10:21:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Apr 2020 10:21:04 GMT
ENV ROS_DISTRO=melodic
# Thu, 23 Apr 2020 10:21:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Apr 2020 10:24:02 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:24:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 23 Apr 2020 10:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Apr 2020 10:24:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b84e9b12c5036e24d270012ffc332ba283c66c65bb1a11c9c36b62ac52c316`  
		Last Modified: Thu, 23 Apr 2020 10:33:34 GMT  
		Size: 9.8 MB (9774901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863092d8428511c061a2c0340a7ec4d93abf5f123245890332e777c71423f808`  
		Last Modified: Thu, 23 Apr 2020 10:33:30 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b36b14c03269a863c72850458f82fa87b8d312d31a723483b3f5702fdc05a2`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2835519f2d237d39236d2dce0f921f1a6dfd9c0631be6c87023f67600d84dcb`  
		Last Modified: Thu, 23 Apr 2020 10:33:48 GMT  
		Size: 62.1 MB (62097551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f60228a5fb4c85cc691071f60a0fc0154ee013df14567edd599f828c3b6ad`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 243.1 KB (243119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00549af9a42e3dd1e9bc8593968eee697343c02e19600216d07d73c9874cc`  
		Last Modified: Thu, 23 Apr 2020 10:34:38 GMT  
		Size: 230.4 MB (230401327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619c48071b4dbff1dd36122924749c4e683b84b45a23f252dd209bc3f04d4ada`  
		Last Modified: Thu, 23 Apr 2020 10:33:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
