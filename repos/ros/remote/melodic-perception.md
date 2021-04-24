## `ros:melodic-perception`

```console
$ docker pull ros@sha256:18fb32103fb1a1223278bfe1988387d642e205ac75ce0061f531df8bec06e04f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6d01605c6f077a6b1481ec73a1961200e6413e060607c6ed175e5b3ea7cb870c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.4 MB (742372640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31900c715089e268c0657f13489c1b03cbbe71a4e623c2335c31fe137025f08b`
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
# Sat, 24 Apr 2021 01:14:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 01:14:43 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 01:14:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 24 Apr 2021 01:14:43 GMT
ENV ROS_DISTRO=melodic
# Sat, 24 Apr 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:18:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 24 Apr 2021 01:18:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 01:18:36 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 01:19:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:19:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 01:20:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:27:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:272f28eb52ac8550b0a48af8b76bda35592d9a4fb09c74ded95b0bbcdb88a131`  
		Last Modified: Sat, 24 Apr 2021 02:05:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b41edd1909d6b6d912dfcfc05f0bc4ccc44ce57d1425a602e63e3302f66348`  
		Last Modified: Sat, 24 Apr 2021 02:06:06 GMT  
		Size: 259.4 MB (259385399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7d49c7d55f79fa7962a3215bf48da8fe904b631a4c0dbdd73def735a6e052d`  
		Last Modified: Sat, 24 Apr 2021 02:05:21 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378afb3fbe3078d5abe9ff0d44d193a1120cefd677d42308510ae16e856e6efa`  
		Last Modified: Sat, 24 Apr 2021 02:06:29 GMT  
		Size: 70.2 MB (70229913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4ff4fe6f504a55e98f8453701f0a87bb1824f6fac9eb68d0679055c648cd43`  
		Last Modified: Sat, 24 Apr 2021 02:06:18 GMT  
		Size: 253.4 KB (253401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c76ffff0385828acb35c2fb381ec500fcf186b7dcea61ae92b76c118d9db40d`  
		Last Modified: Sat, 24 Apr 2021 02:06:33 GMT  
		Size: 75.0 MB (74994793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045826170bdb66e8f1d007621602128be4e8b7c28c278be723bd88136b184d2`  
		Last Modified: Sat, 24 Apr 2021 02:08:01 GMT  
		Size: 305.1 MB (305094346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:4038a7f940468c9ae118140383d50004351116f6d56bb0a1b0a5996966933014
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.6 MB (645596250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e0d03ac7986f63da86619bed965e9067475e6aa6cb560f847b7d013c01d44d`
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
# Fri, 23 Apr 2021 23:32:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 23 Apr 2021 23:32:42 GMT
ENV LANG=C.UTF-8
# Fri, 23 Apr 2021 23:32:43 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Apr 2021 23:32:44 GMT
ENV ROS_DISTRO=melodic
# Fri, 23 Apr 2021 23:36:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:36:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 23 Apr 2021 23:36:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Apr 2021 23:36:19 GMT
CMD ["bash"]
# Fri, 23 Apr 2021 23:37:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:37:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Apr 2021 23:38:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a2c0966898e65c2d9f9c6688597d0a928ac959eb96c75eef346ea75d63a8b75d`  
		Last Modified: Sat, 24 Apr 2021 00:28:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac298ac7fcfc34af628981afad36ad22e9e95c8f1a2a1f3610de71392ad5677`  
		Last Modified: Sat, 24 Apr 2021 00:31:03 GMT  
		Size: 238.9 MB (238867233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e736e949a3520418ea3ad07982372cc43d5012701590be68a2ba3d717f565a1f`  
		Last Modified: Sat, 24 Apr 2021 00:28:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8614e041c3d423b430d489be74e29f19525b525f8815d3a7eafab46f9ee2834f`  
		Last Modified: Sat, 24 Apr 2021 00:31:43 GMT  
		Size: 54.7 MB (54695553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0b25e4f39a13c34d88ea527aba28e66d3176b0a284f9b01a9ee1204982a3b3`  
		Last Modified: Sat, 24 Apr 2021 00:31:12 GMT  
		Size: 253.4 KB (253405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de2a89a3b26efd4329974279c92ef3c198a84bedaea54fceea955165efbe26a`  
		Last Modified: Sat, 24 Apr 2021 00:32:04 GMT  
		Size: 64.7 MB (64744219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f0fc666859f585903cb5cd1ea20ce63b98e73bbdf95a9e7416e1065d526434`  
		Last Modified: Sat, 24 Apr 2021 00:34:49 GMT  
		Size: 259.8 MB (259813764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:103f96d0ee433d7ea9cd21697407d059bea17c407ff6f6db88937c748f3ccd14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.3 MB (703274472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea49bb1148a47a9c4b500f1bcb50cd6d691b44a18928bf5029e3fcd13dd4752`
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
# Sat, 24 Apr 2021 00:23:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 24 Apr 2021 00:23:46 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 00:23:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 24 Apr 2021 00:23:48 GMT
ENV ROS_DISTRO=melodic
# Sat, 24 Apr 2021 00:26:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:27:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 24 Apr 2021 00:27:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 24 Apr 2021 00:27:09 GMT
CMD ["bash"]
# Sat, 24 Apr 2021 00:28:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:28:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 24 Apr 2021 00:29:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1f27d4607596697345ce0405a6ce36d38a3f1eacd4efffdd67b6eee075298c4d`  
		Last Modified: Sat, 24 Apr 2021 01:23:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1400f4e9bf4ad77d4ec4f3e600f380ae67ed173f30586bcdbba70fe42c4038f1`  
		Last Modified: Sat, 24 Apr 2021 01:25:40 GMT  
		Size: 252.3 MB (252328798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bcb83d73f0b6752b4761e171477c587baafae5998cf39a98d63bb5be62ca37`  
		Last Modified: Sat, 24 Apr 2021 01:23:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20f09357d13679ab357353763c43ea18e555ceea6b9388b12caf89776d13aa`  
		Last Modified: Sat, 24 Apr 2021 01:26:14 GMT  
		Size: 63.1 MB (63058129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237a2031202c9603bd619783daaee0037805b151b0fa29780d8781510cc89068`  
		Last Modified: Sat, 24 Apr 2021 01:25:49 GMT  
		Size: 253.4 KB (253405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6631948aad3eff4bff8c7db9301b668a9fd11ceed6beac37dabd75f33a869fcc`  
		Last Modified: Sat, 24 Apr 2021 01:26:28 GMT  
		Size: 67.2 MB (67225080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881a5e500accd020c205097bf5f7a352a50b69fdfdf8b3d9ebb1e3b4d59bc56f`  
		Last Modified: Sat, 24 Apr 2021 01:28:38 GMT  
		Size: 291.4 MB (291407500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
