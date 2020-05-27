## `ros:dashing-ros-base-bionic`

```console
$ docker pull ros@sha256:33071f5742167c2e69101fa5eab9a3d615c2dee62096557759ddce214d194d2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b301c2a59b830c43fbcd6c846864c384fc266b0bbb77a6864e0ed110e264ea7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.5 MB (280476195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fa692c7c4464202ddca4c54711491a6ca9b737233e77f933900d66f0d1c429`
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
# Wed, 27 May 2020 00:45:31 GMT
ENV ROS_DISTRO=dashing
# Wed, 27 May 2020 00:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:47:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 27 May 2020 00:47:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 May 2020 00:47:25 GMT
CMD ["bash"]
# Wed, 27 May 2020 00:48:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:48:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 27 May 2020 00:48:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 27 May 2020 00:48:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:6b37429f6191c8a30c1c62ff7647594e16b6415145b942e005cf2a6dc4a8b83e`  
		Last Modified: Wed, 27 May 2020 00:59:45 GMT  
		Size: 179.4 MB (179409193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a367d9722953d38910e5191d790edc3a4bcc27d16372bfbf892eaca53816406`  
		Last Modified: Wed, 27 May 2020 00:59:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ddc41e729381811da1ef118d91242a3287e98f52da65ec2e28e8bf781cfd2a`  
		Last Modified: Wed, 27 May 2020 01:00:02 GMT  
		Size: 64.1 MB (64139165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d33dd09802f5fd52215082bb7634d7822c89df179456833f25d231167c1ba0`  
		Last Modified: Wed, 27 May 2020 00:59:49 GMT  
		Size: 181.3 KB (181304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58000c3324d41e55f36ea63ee56dccd44871edc87e9601aaa728c6c8f00d0da1`  
		Last Modified: Wed, 27 May 2020 00:59:50 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60a629b4df67fd3f9c0048c71e0649e0d80892a364ad88030a2974cf3409cb7`  
		Last Modified: Wed, 27 May 2020 00:59:51 GMT  
		Size: 4.3 MB (4311731 bytes)  
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
