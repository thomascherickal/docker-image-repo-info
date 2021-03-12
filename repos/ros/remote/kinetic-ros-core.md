## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:ec710af6ce798c65ea37cebebb44a6a444db76fcd1b599cc8841fcfc42052b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9c4ad568301220c7284df3e3f0c5569280f2d0d94557e3d7a9f1318ba44ab728
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.5 MB (238512105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6622d39e7680df31688cbf053a72519e6f2e7b7557a19ca5c41dba4bf0f7b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 13:37:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:37:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 13:37:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 13:37:17 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 13:37:17 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 13:37:17 GMT
ENV ROS_DISTRO=kinetic
# Fri, 12 Mar 2021 13:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:40:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 13:40:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 13:40:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683b460926a81e6b34f03c411843d351a317a876c099ea450473527b8dd9339`  
		Last Modified: Fri, 12 Mar 2021 14:59:06 GMT  
		Size: 5.4 MB (5364270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886f9bb4e8fc7631f82016ca97a031ce164fad541c4cc5338a9c3e448d927c4`  
		Last Modified: Fri, 12 Mar 2021 14:59:05 GMT  
		Size: 14.7 KB (14744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a3c8d2ab08a4cd2184cfa8030b14fa0a848712ae8ad8a5c27a440baaea3b00`  
		Last Modified: Fri, 12 Mar 2021 14:59:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48633ef2719dca18863f07258dc34ec85eb16dec8784b3d40683f5249cba91be`  
		Last Modified: Fri, 12 Mar 2021 14:59:56 GMT  
		Size: 187.2 MB (187168771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed2434900d5d6e5dfa898fc55d491634d1281e686b2111afdc6833046dc93c5`  
		Last Modified: Fri, 12 Mar 2021 14:59:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:953c366addc5e3183add3dedbc96b6079ea090f28674974a4bad305a1db22eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.7 MB (212657019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900e93078c3857b9b8afee0c573c27bae2f6ebc5488c24fd6e98590c354b3883`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:17:15 GMT
ADD file:c77c1a2ea3c8b1d59252626e6c8be57cca539dfce0a16a0ed2ff0311c0f5a265 in / 
# Thu, 21 Jan 2021 03:17:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:17:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:17:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:17:26 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:21:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:21:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 04:21:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 21 Jan 2021 04:21:14 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 04:21:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 21 Jan 2021 04:21:15 GMT
ENV ROS_DISTRO=kinetic
# Thu, 21 Jan 2021 04:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:24:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 21 Jan 2021 04:24:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 21 Jan 2021 04:24:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2af2a813aac2db23328a29ab84155e95fbb6681e872751a4f11f688c005e84c5`  
		Last Modified: Mon, 18 Jan 2021 19:38:27 GMT  
		Size: 40.0 MB (39972659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ef2a276bd8b4a122330892d4a9b9383249f945d22fc34e7b2b0688fbf6af8`  
		Last Modified: Thu, 21 Jan 2021 03:19:28 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c8ce931ce58b3726d3fa387bcf38f02ca4a4d9fa6db2a764bb8aae4f69079`  
		Last Modified: Thu, 21 Jan 2021 03:19:29 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ba02aed017c06ce4541aa061d63a8068bd1651fc0f00b9c0995ec1b22bea3`  
		Last Modified: Thu, 21 Jan 2021 03:19:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d6bcd4fcc109ea638feb11f4efb3cc42368c709239e97d0c80b058d7bac48`  
		Last Modified: Thu, 21 Jan 2021 05:08:43 GMT  
		Size: 4.6 MB (4615362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dada356e54fac0aeb0fc744ccbca68ed154ef97d589d1a9b2e810dab83264c6`  
		Last Modified: Thu, 21 Jan 2021 05:08:41 GMT  
		Size: 14.7 KB (14744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b25c03a830017441e51bb0ee2af49968aa6de63b2d1c8dc15c295e3a71c60`  
		Last Modified: Thu, 21 Jan 2021 05:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dfd6725ae662c908d1df455362722a807ff5ce1dd3f66e0356c7fc3cba8f9a`  
		Last Modified: Thu, 21 Jan 2021 05:09:44 GMT  
		Size: 168.1 MB (168052304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe4dcfe4ec1442358eef15e27bdb52616942a46251eeb5e16c05e6e01fc7abe`  
		Last Modified: Thu, 21 Jan 2021 05:08:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:39186c19b9e2ccfa8e6ca3d0361898a5e4351b78a3ddd936885b020cbffb67cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221744699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6fa6513cb709b0cb5cc095244c4a21bcb48b9816ce78f0ceece70e5c9e15f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:27:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:27:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 06:27:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 21 Jan 2021 06:27:09 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 06:27:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 21 Jan 2021 06:27:11 GMT
ENV ROS_DISTRO=kinetic
# Thu, 21 Jan 2021 06:29:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:29:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 21 Jan 2021 06:29:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 21 Jan 2021 06:29:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0596a8732aadbc8704f74fca2d9a1a5a769d11c968c46103f313b03d4d5cd68`  
		Last Modified: Thu, 21 Jan 2021 07:22:49 GMT  
		Size: 4.8 MB (4820293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbda91611b700613684e2b08b7cb4c1ce1b58c152f34838d51f2b320ceef983`  
		Last Modified: Thu, 21 Jan 2021 07:22:48 GMT  
		Size: 14.7 KB (14744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2b1318bd99b208ca1a2d36788e661df11ae80e5a774b26095bd70e517a8873`  
		Last Modified: Thu, 21 Jan 2021 07:22:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8a247eee41c59c7799a7f9b83a86a04c4be4fb946d8b463b5f1f12b52b36fb`  
		Last Modified: Thu, 21 Jan 2021 07:23:36 GMT  
		Size: 176.0 MB (176022535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c81e12c5a66cd90daa8379fbca97b6a27b3005b29c5a698d1b6ef8ce185a`  
		Last Modified: Thu, 21 Jan 2021 07:22:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
