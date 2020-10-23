## `ros:noetic-perception`

```console
$ docker pull ros@sha256:7ed02ca5bcc5861f9e97b125e956206bc29bc2f8d124f9b83e6522514d433365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:71d62272830e9cbfc6c3a20dd8e6369d013d323717e0b580dcb491a99df4f0af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **806.1 MB (806103498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed82a3bc0da9d9efaca3e6d5c0bba95bd513c05fc33c2bc7e70f7b6c8aca544`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:36:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:39:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:39:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 19:39:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 23 Oct 2020 19:39:28 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 19:39:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 19:39:29 GMT
ENV ROS_DISTRO=noetic
# Fri, 23 Oct 2020 19:41:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:41:34 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 23 Oct 2020 19:41:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 19:41:35 GMT
CMD ["bash"]
# Fri, 23 Oct 2020 19:42:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:42:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Oct 2020 19:43:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:49:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff1f5aa6532e89f99088e3f051edc77e327f1be209cae1a67a9a4a9d75ab918`  
		Last Modified: Fri, 23 Oct 2020 19:57:00 GMT  
		Size: 1.2 MB (1176911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ea0b4003c131677032f1b780e81fe1340558bdda164da50e8dc00028e8fe99`  
		Last Modified: Fri, 23 Oct 2020 19:56:58 GMT  
		Size: 5.5 MB (5547520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff461b03c5c5f446813ac962f11e949edf73b550d9ae717ba14ba7ce61a8d38`  
		Last Modified: Fri, 23 Oct 2020 19:56:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b31ccc19a2b1cb24c2139e385f18a03225840908a49cc712267689d867a80b`  
		Last Modified: Fri, 23 Oct 2020 19:56:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7b0e1d10adc8821b6deb0a1a21160f6081d359c111f5b20bcf6fec8fc10188`  
		Last Modified: Fri, 23 Oct 2020 19:57:44 GMT  
		Size: 173.3 MB (173254471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4151be45037971b76077bd93c94b9a8b7988c5951cf6ee6e2b6c9294cfe5ae5`  
		Last Modified: Fri, 23 Oct 2020 19:56:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e4a7c0cf1a7bad6b87239dc4a8ec2ac115f2d6effb7fc8173af2abef068b68`  
		Last Modified: Fri, 23 Oct 2020 19:58:10 GMT  
		Size: 46.4 MB (46381120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e3683912f49b138110ce9b53ccc203afea17e6e87906ada2cb66b9a04206ac`  
		Last Modified: Fri, 23 Oct 2020 19:58:00 GMT  
		Size: 244.2 KB (244190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92250d9cc0c56021f33ebad01007d8455c557630943cf2b72a82ae557a2bda2a`  
		Last Modified: Fri, 23 Oct 2020 19:58:16 GMT  
		Size: 79.6 MB (79590370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf7928ce5282eaef02d6c8be5fa622aa7d373044e1d7032e5552384dbd05f1b`  
		Last Modified: Fri, 23 Oct 2020 20:00:07 GMT  
		Size: 471.3 MB (471347358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:d48b6e795c218610506bacbfa633fdc622f77a2c614360a55b4fb21ad2f3fae5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.1 MB (702079711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a745eca878aac68c41ad22016d56277699af916fd48d1dbcada75ab35f393ab8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 18:16:23 GMT
ADD file:7eef4725b8e0594e6d033da471b98f508fde3df29100aa6cdc33180d4524cf62 in / 
# Fri, 23 Oct 2020 18:16:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:16:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:16:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:16:30 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:04:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:04:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:04:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 19:04:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 23 Oct 2020 19:04:29 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 19:04:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 19:04:31 GMT
ENV ROS_DISTRO=noetic
# Fri, 23 Oct 2020 19:06:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:06:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 23 Oct 2020 19:06:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 19:06:37 GMT
CMD ["bash"]
# Fri, 23 Oct 2020 19:07:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:07:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Oct 2020 19:08:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3c478921ca13a317a5584d4f9ec27e1688931fcc71a74949622ecd0dca63baa`  
		Last Modified: Mon, 12 Oct 2020 16:20:05 GMT  
		Size: 24.0 MB (24039636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98985506b7e726afa2b8d178a88ffec8b51c3ae9d7f6f11279e5000c808761e`  
		Last Modified: Fri, 23 Oct 2020 18:17:41 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd88c4be5a76e00881f4097c47a3db7ea802048fb9e329475381f78c0ce82767`  
		Last Modified: Fri, 23 Oct 2020 18:17:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b963526a7df71b7e05c0adf371402eeeb5bd59c00fbb8aca3a5412e7a18845`  
		Last Modified: Fri, 23 Oct 2020 19:19:05 GMT  
		Size: 1.2 MB (1178174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8190b94afd6d9978079c7724a5a21a3494bb87eaf3c7d7cd631448bdad4ff79`  
		Last Modified: Fri, 23 Oct 2020 19:19:02 GMT  
		Size: 4.7 MB (4676700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adfccc960d05022f884aee23f9834396b4e3e15c482e5cb4582267e3efa76d0`  
		Last Modified: Fri, 23 Oct 2020 19:19:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d72cdef4b65ab2bc256577cd06f4be746e2ca7fcd152ba303ccd3c93c622fa`  
		Last Modified: Fri, 23 Oct 2020 19:19:01 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fc7b934d345f2ebf5bce0b55302c6b2579796c6d2495cbccd48a2b27cb1495`  
		Last Modified: Fri, 23 Oct 2020 19:20:01 GMT  
		Size: 157.1 MB (157132123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3706aa3752b25a7c7d5c10f1817ef4a857482a43b0a621b68443b70eada63c97`  
		Last Modified: Fri, 23 Oct 2020 19:19:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d9124886128adf14c7447ca57ad9003ace8830e72a5671d540834b31583705`  
		Last Modified: Fri, 23 Oct 2020 19:20:20 GMT  
		Size: 35.8 MB (35830286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4eaafd2ab89a73dee5b3723b170b2697911b80ad43fa35dd09c268b5cca3de`  
		Last Modified: Fri, 23 Oct 2020 19:20:10 GMT  
		Size: 244.2 KB (244247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c905c798bfc98b1be79903450ee61c8c93cb970d8f97fc3a68ad52641e33912`  
		Last Modified: Fri, 23 Oct 2020 19:20:31 GMT  
		Size: 60.5 MB (60482364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9ab555c70b4d5a597d163b13be653496c81fac7232eb296dbb24dd777dc516`  
		Last Modified: Fri, 23 Oct 2020 19:23:13 GMT  
		Size: 418.5 MB (418493303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ca6485e9850877f19067a176f736a72b80ac810e9424ccc95a8c128115bed4d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **758.5 MB (758454936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca42a9e65a8024486dba8203dd4ae063325c5ae131350ede00167e96eeaf1cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:06:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:06:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:07:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 19:07:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 23 Oct 2020 19:07:04 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 19:07:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 19:07:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 23 Oct 2020 19:09:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:09:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 23 Oct 2020 19:09:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 19:09:08 GMT
CMD ["bash"]
# Fri, 23 Oct 2020 19:09:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Oct 2020 19:10:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a57a33cfa330c14ee308343f9e2a73382a99ccf08c3c905dbb22831ec69c86`  
		Last Modified: Fri, 23 Oct 2020 19:24:02 GMT  
		Size: 1.2 MB (1178042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c463e5d0fb6cd5bb763e1856a0ca0db13a28b7a5ff531cf5ea2a2d778ab6e536`  
		Last Modified: Fri, 23 Oct 2020 19:24:00 GMT  
		Size: 5.5 MB (5513934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7a377b36c34d24c6e2a5c5a7f9cbcfad3511145bdf413951e31feedfadd819`  
		Last Modified: Fri, 23 Oct 2020 19:23:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a582741bbbe4b4ce1be6bad001cde2b793e50706f5e90e8b36d23f19c14ca0`  
		Last Modified: Fri, 23 Oct 2020 19:23:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70d1136be82e1ce8f601728260d0c09313afee99bf26742537a3093698897b4`  
		Last Modified: Fri, 23 Oct 2020 19:24:48 GMT  
		Size: 167.7 MB (167700155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2511dc3e97b985ee4f4331691dee016a2e9be3623d0c81695375d89c01c0d60b`  
		Last Modified: Fri, 23 Oct 2020 19:23:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d446f5fc799b5e6b4902e1b2cae2026ea6eca5913b78a5869f8a304380e950c4`  
		Last Modified: Fri, 23 Oct 2020 19:25:05 GMT  
		Size: 40.7 MB (40651238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877662818fc66a00d3eb4dce7349c1ad289efad353ef97a34699ecd0e60f757`  
		Last Modified: Fri, 23 Oct 2020 19:24:55 GMT  
		Size: 244.2 KB (244249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ddd0a924640d0a9fb60133cb0c2a33a87af4bff2be10da74d18f5697a633fc`  
		Last Modified: Fri, 23 Oct 2020 19:25:31 GMT  
		Size: 72.0 MB (71973891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ff4445b2eed316ca2a3915fff52cbe3bc08b36d8e40bf3ec9652ce4b0a1bc8`  
		Last Modified: Fri, 23 Oct 2020 19:27:57 GMT  
		Size: 444.0 MB (444026713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
