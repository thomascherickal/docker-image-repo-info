## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:c11823d856edb73de81178998925b594ed355f00c04e72fec120f44fd7135395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:d6064a191f4d05536906c70d383bb7d6b9dc68d968f2d8421d0142c85df22f77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299847099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da2c79c08d094f07f08b9be029bcd7f4c87cad533917662552e50cbc2d61a26`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:5d0ba1e209a87319c13c0dcc46624885b70f03aefbe4d674264c6bedadacd287
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260283861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7d0e47b5d227a696151c6dcb03c7d8127acdc3ef603e7317b1328604638ada`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9ef434329904a1e126b6be2a29fd78634640f3417a178cbffd08cd14bd574bc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272599287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db694db52cb9b174d57d38ba2b52b6de66f29c1c1212adfad963c71470783bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
