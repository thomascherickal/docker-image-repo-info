## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:c26afd5a8523a07f33ceac44e7acc8e2da16e075170e8d7e7d8fb590c4370d1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:f3fca116206a2d694cdb30dc2cf8809221fa13cf26e2d7052650e2cc1c97b7fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208614185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c270e8b844876c63999942d26dcf453411f24c4a2f37409a325e4494a946058e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:39 GMT
ADD file:c77338d21e6d1587df92d76a2b0a5c36f0e026ac1640b5cddefb1bf8db8a1204 in / 
# Thu, 04 Mar 2021 02:24:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:42 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 10:03:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:11:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 14:11:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 14:11:56 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 14:11:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 14:11:57 GMT
ENV ROS_DISTRO=noetic
# Fri, 12 Mar 2021 14:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:15:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 14:15:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 14:15:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5d3b2c2d21bba59850dac063bcbb574fddcb6aefb444ffcc63843355d878d54f`  
		Last Modified: Mon, 22 Feb 2021 16:09:51 GMT  
		Size: 28.6 MB (28567785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2062ea6672189447be7510fb7d5bc2ef2fda234a04b457d9dda4bba5cc635`  
		Last Modified: Thu, 04 Mar 2021 02:25:50 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf526d75b82eb4f9981cce0b23608ebe6ab85c3e1ab2441f29b302d2f9aa8`  
		Last Modified: Thu, 04 Mar 2021 02:25:50 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cfec6f2da960164171c5970a0a257d0cedb5f791a43019ec06be3f6be3842`  
		Last Modified: Fri, 12 Mar 2021 10:28:38 GMT  
		Size: 1.2 MB (1182808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694590d03abf5d1734a02addbf98c8bae4b3ad1ebdf9523ec5687888462f1360`  
		Last Modified: Fri, 12 Mar 2021 15:09:45 GMT  
		Size: 5.5 MB (5547975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b6051fbcd3c71d56397c8f01cf7b807b358b76dfbd34be6f585e364b69645f`  
		Last Modified: Fri, 12 Mar 2021 15:09:43 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc8133533ae89e3ad614bc429a30e18ef7d259d07108d425131781c318aaf8`  
		Last Modified: Fri, 12 Mar 2021 15:09:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82185e13c9689d76552222b09e4ab0bd998e91948ed05a1671e793ab89d25ad`  
		Last Modified: Fri, 12 Mar 2021 15:10:29 GMT  
		Size: 173.3 MB (173312769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000d14daeac3082225cbc7d71ef45f036e309d6a268af14dced6da654299fc49`  
		Last Modified: Fri, 12 Mar 2021 15:09:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:7363a8130a80aecac76c1a2e2721df36d3e731fef95a4ac8d8de6aa0cb430eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187080863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374e2f38a8e7592b2117370885e49e5ae50a29b44bf41a1750dc279d7cd31903`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 03:11:51 GMT
ADD file:d804f9669b02065930f45cd4dd689caac310feee2f838826a1019e46431531e0 in / 
# Thu, 04 Mar 2021 03:11:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 03:11:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 03:11:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 03:11:59 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:14:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:14:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:14:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 04:14:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 04 Mar 2021 04:14:37 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 04:14:38 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 04:14:39 GMT
ENV ROS_DISTRO=noetic
# Thu, 04 Mar 2021 04:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:16:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 04 Mar 2021 04:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 04:16:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e0e04e4d364e7a1732453d9002fa463c863601b22f0a6590507d5659740246e6`  
		Last Modified: Mon, 22 Feb 2021 16:17:35 GMT  
		Size: 24.0 MB (24046119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7c5587c59a45992952b809737c49f286368858bca445206d3e194fb0ec89c3`  
		Last Modified: Thu, 04 Mar 2021 03:13:31 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f1be617f9f5a055e4a8885c56e5a09e67171bb42a97a0f8ce2e9a3af77f12`  
		Last Modified: Thu, 04 Mar 2021 03:13:31 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83d21742e73765e5f38c2d54750062c57bec9ca4ae084a92780f29c41e3504f`  
		Last Modified: Thu, 04 Mar 2021 04:44:22 GMT  
		Size: 1.2 MB (1183137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3983cd9f6e8b3ccf950d2c1fce56a69be5ac635c2b4468159619c542768bd217`  
		Last Modified: Thu, 04 Mar 2021 04:44:21 GMT  
		Size: 4.7 MB (4676789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628d4754ef261e2fddf499b687ee5e6d158d94071b0377158bdcc0d75901fc9b`  
		Last Modified: Thu, 04 Mar 2021 04:44:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e988973cd6210797d1e014a729201525cb147bf3f775fdc0bc6897184e3a2c42`  
		Last Modified: Thu, 04 Mar 2021 04:44:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac148e3c471d0b7cfd4e76973e0d0501ddedfd6b132c3c2ac16507c33fb72bca`  
		Last Modified: Thu, 04 Mar 2021 04:45:20 GMT  
		Size: 157.2 MB (157171939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64087840f298da17ccc82c616eeab994eaab7dfc6360297c3f798eed8ca9cf57`  
		Last Modified: Thu, 04 Mar 2021 04:44:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5e2a44883f3fc8e03d9c5df0d90fdac182b9146e917960bfb9b41bdceab95641
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.6 MB (201620636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307adab9e47ce7a3af5e2a61d3530fe0b3b707d3786b593299ff8b333270ee72`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:52 GMT
ADD file:1dfda258a4ebfa53687877ae153107d2e472e0b039363ec35aafe9f5733cae22 in / 
# Thu, 04 Mar 2021 02:52:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:53:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:53:01 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:22:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:22:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:22:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 03:22:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 04 Mar 2021 03:22:39 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 03:22:40 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 03:22:41 GMT
ENV ROS_DISTRO=noetic
# Thu, 04 Mar 2021 03:25:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:25:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 04 Mar 2021 03:25:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 03:25:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:32d7611b468cbc07986302f1a8e74d92e30a1f11cdfa8bc2900aedda2758d050`  
		Last Modified: Wed, 17 Feb 2021 08:25:24 GMT  
		Size: 27.2 MB (27175799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be16fdc30614524222cdec466297e7ed49c7695e868c5dd2700a1778d88b23`  
		Last Modified: Thu, 04 Mar 2021 02:54:33 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a361e87bde5e27ceda037ab2116d88d9570b6d53c34102a2a214ef2944270138`  
		Last Modified: Thu, 04 Mar 2021 02:54:34 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1317e878738b2e361ab2bc6c5e9dad3effcdd7f83f6a2e3687fc82bc9c1ada3`  
		Last Modified: Thu, 04 Mar 2021 04:04:00 GMT  
		Size: 1.2 MB (1182875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba5f746c529c10d1d08e23f12a45a07e2921c194edd5618c4b72f862233e909`  
		Last Modified: Thu, 04 Mar 2021 04:03:59 GMT  
		Size: 5.5 MB (5512834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea8b4c459768d7eb6fc2a16d12531aface693a3d22b366e35336593ee89d6ad`  
		Last Modified: Thu, 04 Mar 2021 04:03:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eecb3e613c32cdcaf95e9ff1c2bca8076ca8109c82abc46aaac30fdda393f88`  
		Last Modified: Thu, 04 Mar 2021 04:03:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2abe5add42bec709ddb08a5174fb61aa16a17e0172cd3cb8efb6e1f0542d55a`  
		Last Modified: Thu, 04 Mar 2021 04:04:49 GMT  
		Size: 167.7 MB (167746250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec9fcc6dbe4e86533f2c0fec339f14a7acaf1dff8dd8b877e0b5f9edb2d6ba`  
		Last Modified: Thu, 04 Mar 2021 04:03:58 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
