## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:b319bc6aa9bfd70ee90a47e4e89221bb98200df912dbd069fa276e2560f46231
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:1c004ac6f6f0edef08423ffeaf0407a5d5b53cf85173d2794cd37dc001e742b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **682.4 MB (682444049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:851ccc9b3d528ef0aab5d9a968e9cef5942f2532135784eeb45ef1fa5accc27f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:04:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:04:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 18:04:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Jul 2020 18:04:56 GMT
ENV LANG=C.UTF-8
# Fri, 24 Jul 2020 18:04:56 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Jul 2020 18:04:56 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Jul 2020 18:06:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:06:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Jul 2020 18:06:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Jul 2020 18:06:57 GMT
CMD ["bash"]
# Fri, 24 Jul 2020 18:07:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:07:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Jul 2020 18:08:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:11:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35d3e490359bfb27251001813204a784160c727634421f0c2e9dfa17b6fb0d8`  
		Last Modified: Fri, 24 Jul 2020 18:49:13 GMT  
		Size: 5.4 MB (5362308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b88a1122f09c1c0c1f8013020bb517e065fb454ee14c9198d0ebc81e8eb178`  
		Last Modified: Fri, 24 Jul 2020 18:49:12 GMT  
		Size: 14.7 KB (14742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56fd6ccab8aa88dd0da1a26c17d9d16c360babbbcf79c5053f83e8a9ede3c20`  
		Last Modified: Fri, 24 Jul 2020 18:49:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b3ea9059f6170d73a2f76687f4bc2cba92bf7a31a9c70945c59bce1ac727d6`  
		Last Modified: Fri, 24 Jul 2020 18:49:55 GMT  
		Size: 187.1 MB (187146511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9ccf49031078286631b1c695648fbbd1128e27b5fad0b31e8b09163e130516`  
		Last Modified: Fri, 24 Jul 2020 18:49:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d029ddd3bef6066e72480266b88b12f62ee39e09d1ac6e1421c48b28ec0b71c3`  
		Last Modified: Fri, 24 Jul 2020 18:50:12 GMT  
		Size: 57.2 MB (57240491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4ee9e9576e4d6e20a9550a0770f506c30f59dc98accc213ef7c767df669ce8`  
		Last Modified: Fri, 24 Jul 2020 18:50:01 GMT  
		Size: 261.6 KB (261579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933ab14125779e7659d132b8fc94f05d5d82bfca5860c5d0739e574b1ea3c1dd`  
		Last Modified: Fri, 24 Jul 2020 18:50:15 GMT  
		Size: 63.6 MB (63572296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dfef674dc4a341b8abb14137bf27abe1dc588281998e99b06c918eb9009860`  
		Last Modified: Fri, 24 Jul 2020 18:51:35 GMT  
		Size: 324.4 MB (324443137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:07cc80d2dbc539272a35144173431f49e62807d57ae5fbd812c7af2a9c09755d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.5 MB (576526411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e75d2f5884c58b63c7b8f3c34fe06180ef4426c42a6b38d0f392f15927b4947`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:46:44 GMT
ADD file:0b278cf0607b320084ec5b7202c2165582b90918197e7c7a3b6f5a978b67dac7 in / 
# Wed, 19 Aug 2020 21:46:49 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:46:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:46:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:46:54 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:29:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:29:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 22:29:31 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 Aug 2020 22:29:31 GMT
ENV LANG=C.UTF-8
# Wed, 19 Aug 2020 22:29:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 Aug 2020 22:29:33 GMT
ENV ROS_DISTRO=kinetic
# Wed, 19 Aug 2020 22:32:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:04 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 19 Aug 2020 22:32:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 22:32:06 GMT
CMD ["bash"]
# Wed, 19 Aug 2020 22:32:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:33:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 19 Aug 2020 22:34:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:38:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fb84101310d5621e3be19975c1bb24b9f684f7ffec110cb3d4982441c388a96`  
		Last Modified: Mon, 10 Aug 2020 14:27:50 GMT  
		Size: 39.0 MB (39047599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb62b8b664ef29d7c2413ebe2c638345e086b0c0519560854eae02c7e1c873bf`  
		Last Modified: Wed, 19 Aug 2020 21:47:57 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d891ce98e9b325ec87d26f9bb78ce486bb420846e496514de1af5e588b43404`  
		Last Modified: Wed, 19 Aug 2020 21:47:57 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361ed46998eb1705595b9fada81f47ab2ace3728bdd2f497680f5e8480b77530`  
		Last Modified: Wed, 19 Aug 2020 21:47:57 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100dec9138b3098e55244cce8dc401d1b7dc0a5e6530daf3a78ef27c3322c9e`  
		Last Modified: Wed, 19 Aug 2020 23:15:27 GMT  
		Size: 4.6 MB (4615382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc7b35d7dd6df61d7c29c9c48efafbe84bc9abb3e27af740040976a027ae5e5`  
		Last Modified: Wed, 19 Aug 2020 23:15:25 GMT  
		Size: 14.7 KB (14743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309e1fe0a6f12fe4fd6243e317127b78f852d62f0cb9893ef8826d30b2527ca1`  
		Last Modified: Wed, 19 Aug 2020 23:15:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c901563883e0c6209f4c05d161f953dd02bf08f2410a550fef06ef2634216c67`  
		Last Modified: Wed, 19 Aug 2020 23:16:22 GMT  
		Size: 168.0 MB (168009545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2ae779ec22740f850ccda71035491712275550dff2be9f7a24b8ab8c69c008`  
		Last Modified: Wed, 19 Aug 2020 23:15:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42656b198f53fb5cee1885331b56023d373c943f3be84cc1bef7fa854763f419`  
		Last Modified: Wed, 19 Aug 2020 23:16:41 GMT  
		Size: 42.9 MB (42892355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b8a791f8a2b69215074add4a2a2eb949978df149fb36ba1041cdc0567b0c6`  
		Last Modified: Wed, 19 Aug 2020 23:16:29 GMT  
		Size: 262.8 KB (262848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef35062d493611d95eed66d1aca062dfd283a3bbe9878be1097de13d0214afab`  
		Last Modified: Wed, 19 Aug 2020 23:16:46 GMT  
		Size: 55.5 MB (55500384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eac6f178d3c8d4e6a84a3bf14b7415efc0eeaffc006ed5d4ed6d054e31493c`  
		Last Modified: Wed, 19 Aug 2020 23:18:30 GMT  
		Size: 266.2 MB (266181598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:277e82f4189506ee0a03c5ac7879af2f5ea0f73050859499a5e51e21dbdbbc05
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.1 MB (600142912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edce86c3560da2f6812f3154eb930b805ac5e4f14a626facd1294cb5d17b43e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:25:59 GMT
ADD file:d816988decfebf469e2b28b4858ce7d4a991a101957a43051324255fbe64c86e in / 
# Fri, 24 Jul 2020 16:26:14 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:26:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:26:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:26:27 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:31:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:31:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 16:31:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Jul 2020 16:31:10 GMT
ENV LANG=C.UTF-8
# Fri, 24 Jul 2020 16:31:11 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Jul 2020 16:31:12 GMT
ENV ROS_DISTRO=kinetic
# Fri, 24 Jul 2020 16:36:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:36:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 24 Jul 2020 16:36:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Jul 2020 16:36:50 GMT
CMD ["bash"]
# Fri, 24 Jul 2020 16:37:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:38:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Jul 2020 16:40:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:45:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f783735449ae0b09fb9e5ee128904f2f3131f6ba46fcf1350fb6a10f872866be`  
		Last Modified: Tue, 07 Jul 2020 00:25:09 GMT  
		Size: 40.1 MB (40050796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35a03aa6fbe0d9147b23501e6fa41d33cd4489470455008ddcbe201063d7b98`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55e221892467d43fdd76b2b592c2fe46e1c69b08e0e9b94f2b383f38e681f65`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a9069021914a77a3d51ffbff02ea5b8a200180601b2be52e9f98d31b6f1389`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406ac69f173003c8bf0c008eaef291209c10ae7cd840633b6dfa0c3351a3c19a`  
		Last Modified: Fri, 24 Jul 2020 17:38:25 GMT  
		Size: 4.8 MB (4820044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9658dddd254b3a9732e5e0eff70e9f0c4ca573b2ffb9d7031fa9a89c1b99c518`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 14.7 KB (14745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e008049660c6d8aae525a64b5fba4a4b918e212cc2548f8b1e35eb7a1cc35e41`  
		Last Modified: Fri, 24 Jul 2020 17:38:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b3f6f90a52db94535a8a10507e8b9981b17dddce080db1b8f558a66fdb497a`  
		Last Modified: Fri, 24 Jul 2020 17:40:19 GMT  
		Size: 176.0 MB (175982202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4782a0457e8a49bdd7b6d2f7935bf248fa8eb8dc68b418fdab6e7edccf157cb7`  
		Last Modified: Fri, 24 Jul 2020 17:38:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7882cb49935fa348f0e3b473d812599196078588f2ce8478a4a3959bd6c4ec04`  
		Last Modified: Fri, 24 Jul 2020 17:40:56 GMT  
		Size: 46.0 MB (45953072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd7eff6b60a1b27641649ad49d8a67a7db88cbd74871b4e32b1c8280d7f561d`  
		Last Modified: Fri, 24 Jul 2020 17:40:32 GMT  
		Size: 261.6 KB (261629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e031cb5a1d31714b1b1f232b00b326ef1cf62133cea749e67154d808097533f`  
		Last Modified: Fri, 24 Jul 2020 17:41:04 GMT  
		Size: 57.3 MB (57286641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f728b1a8a3b623f496cc939ba1bfbf75160e446b0ca9ae822b08b054fa84ef3`  
		Last Modified: Fri, 24 Jul 2020 17:43:37 GMT  
		Size: 275.8 MB (275771871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
