## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:4c660325b730c508ebf44a3bb7706c95da01e08da878374617f2c4b849ccfe29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:ee955a0b2def55120d9345dcda1b123d90a3c8c45bd1ee37fbbb5ae04ab20c8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.8 MB (350758659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c383b6649e02f6a29821b9eeb5d63c9c0f6c0a9cffcfb0e940362c16cb9dd8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:08:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:20:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:20:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 02:20:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 03 Apr 2021 02:20:44 GMT
ENV LANG=C.UTF-8
# Sat, 03 Apr 2021 02:20:45 GMT
ENV LC_ALL=C.UTF-8
# Sat, 03 Apr 2021 02:20:45 GMT
ENV ROS_DISTRO=noetic
# Sat, 03 Apr 2021 02:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:23:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 03 Apr 2021 02:23:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 03 Apr 2021 02:23:03 GMT
CMD ["bash"]
# Sat, 03 Apr 2021 02:23:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:23:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 03 Apr 2021 02:25:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:25:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c5d2d7a6606006c3c9ad68491e77516419c59fceb2f4c04ca5580c96d8501`  
		Last Modified: Sat, 03 Apr 2021 02:40:16 GMT  
		Size: 1.2 MB (1182070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccd2266e6deaba5ba5682d19318df74543102cf36e0b3e2be8240cbd58404eb`  
		Last Modified: Sat, 03 Apr 2021 02:40:15 GMT  
		Size: 5.5 MB (5547325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2974076651535b81ed47daec0c9ac8a8a614de3b86c54d48a04c89ad19e07559`  
		Last Modified: Sat, 03 Apr 2021 02:40:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeea5a3064223d136dad685d029154144e0901ca9a3ee89a6195cac489b5f2be`  
		Last Modified: Sat, 03 Apr 2021 02:40:13 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edc3a0a092cee09a3ffdb2b7b19f0ba9493b6b89e67ba30c41a5832469ab736`  
		Last Modified: Sat, 03 Apr 2021 02:40:51 GMT  
		Size: 173.3 MB (173295914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3697162c286ff1061f7806c84cd1eb621e8cae61d469f5b680e7e85dfb0d2eb`  
		Last Modified: Sat, 03 Apr 2021 02:40:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a97757554a359d2bb282b36def792eaf90c8ac425a7f31f8cbf7eb1a4e00d7f`  
		Last Modified: Sat, 03 Apr 2021 02:41:12 GMT  
		Size: 46.4 MB (46384019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dce28915494b4ad3c2b27b876af19e0231c6c6d7e43563953c4a12ab21aba9`  
		Last Modified: Sat, 03 Apr 2021 02:41:03 GMT  
		Size: 281.4 KB (281381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ad59c3114105ea5f83161a8463d13c8f995bd4af249a920444b681b47b833`  
		Last Modified: Sat, 03 Apr 2021 02:41:17 GMT  
		Size: 79.6 MB (79599777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b330ffc0c351e858d64d7a01f13dab1ed881e3d00f50d308169f50e10816cc1`  
		Last Modified: Sat, 03 Apr 2021 02:41:34 GMT  
		Size: 15.9 MB (15896287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:088b8696adccf6cd458f2306fd095ac160b3e0ac03c721b79bde9ba6ac7d07b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297749052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae14dde2993b342da7f48731d487d8f6ff29b94e9f0b08928710a2d0102a7ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 03 Apr 2021 01:42:07 GMT
ADD file:76d0a7f82466172411203f4c90d7ec41979ea48db42fa3dd8a53f15622612f6e in / 
# Sat, 03 Apr 2021 01:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 01:42:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 01:42:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 01:42:15 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 03:21:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:21:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:21:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 03:21:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 03 Apr 2021 03:21:41 GMT
ENV LANG=C.UTF-8
# Sat, 03 Apr 2021 03:21:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 03 Apr 2021 03:21:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 03 Apr 2021 03:23:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:24:00 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 03 Apr 2021 03:24:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 03 Apr 2021 03:24:01 GMT
CMD ["bash"]
# Sat, 03 Apr 2021 03:24:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:24:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 03 Apr 2021 03:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:26:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b310eb6279419eece82e847effefb67be66a3b8e631fda5532880177728460e`  
		Last Modified: Fri, 02 Apr 2021 12:47:42 GMT  
		Size: 24.0 MB (24048394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051c3059c680dcb64b0535e921132c5c74999d067a3eee05538c186b50546bb5`  
		Last Modified: Sat, 03 Apr 2021 01:44:02 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0927a80501a33ba38863296941a21c086fe86d55e066d7b4095548ef7e2a17e3`  
		Last Modified: Sat, 03 Apr 2021 01:44:01 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac06057a67e37c332e7b8402c6abb43271e4ec608389364d844259b500aaea`  
		Last Modified: Sat, 03 Apr 2021 03:32:15 GMT  
		Size: 1.2 MB (1183300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94542727c4711006f6f1782a08cd205bc3c1e45341f1b336bad762cbf4f0f596`  
		Last Modified: Sat, 03 Apr 2021 03:32:14 GMT  
		Size: 4.7 MB (4677018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09d8fc11106bdfeb8785801ebd429ce7d8aaf07041c5042303b64ac169aee68`  
		Last Modified: Sat, 03 Apr 2021 03:32:13 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03297d605a86b508fdf31f52053570edf2ad44479187c2108aefeb991fffc94a`  
		Last Modified: Sat, 03 Apr 2021 03:32:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495387802583f80d489a3eadb721ee2311ff8a4de110530efa6cf22a41f34cb7`  
		Last Modified: Sat, 03 Apr 2021 03:33:12 GMT  
		Size: 157.2 MB (157156555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6713d05fef74e96cff45d8374c53a4958974189685140fc4076a3b35b10edb`  
		Last Modified: Sat, 03 Apr 2021 03:32:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc51d1bdf316d5930c657790042bc61c7ac329c5bb56b16bd4c96edbe067d8e0`  
		Last Modified: Sat, 03 Apr 2021 03:33:30 GMT  
		Size: 35.8 MB (35832675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e23ba0364adac106b1f028b91e13f1b10769d62d6d9709f58f9b7a7f46a846`  
		Last Modified: Sat, 03 Apr 2021 03:33:19 GMT  
		Size: 281.4 KB (281385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c079bbcf301a105f7e1be1389c761371f9ece7cbbe5eb3dae1b9247b846f71`  
		Last Modified: Sat, 03 Apr 2021 03:33:42 GMT  
		Size: 60.5 MB (60478983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c79709d1a0ea264ca2ab9f9c1ad7f216c51fa1a8f7dba6ba62d7343b89bcdde`  
		Last Modified: Sat, 03 Apr 2021 03:33:55 GMT  
		Size: 14.1 MB (14087867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8a105b3a4933d3bc4a0c848d1174e52493fc2b73efa403d6b2d27be363eabc86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.0 MB (329995607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72437af4c70266ff3401761d970ea6f0e90903a2088ed245b6703efda713474e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:25:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:26:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:26:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 06:26:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 03 Apr 2021 06:26:13 GMT
ENV LANG=C.UTF-8
# Sat, 03 Apr 2021 06:26:13 GMT
ENV LC_ALL=C.UTF-8
# Sat, 03 Apr 2021 06:26:14 GMT
ENV ROS_DISTRO=noetic
# Sat, 03 Apr 2021 06:28:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:28:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 03 Apr 2021 06:28:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 03 Apr 2021 06:28:16 GMT
CMD ["bash"]
# Sat, 03 Apr 2021 06:28:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:29:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 03 Apr 2021 06:29:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b425e160ecdc1ce2e8f2c9394df0bf787e591ab7983fa386fa029ed26a92c1`  
		Last Modified: Sat, 03 Apr 2021 06:48:05 GMT  
		Size: 1.2 MB (1183308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19dbee98155e4cab1ca612d6d81cf3e8713fb2f87fc42d92530e2635fd1ba8f`  
		Last Modified: Sat, 03 Apr 2021 06:48:04 GMT  
		Size: 5.5 MB (5513345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874fc4821a261dd3d76266f77f06518b341b2bea50a79bd0dbc4fd367823c520`  
		Last Modified: Sat, 03 Apr 2021 06:48:03 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea4fc90e4b6b3da2ae41f950759083412f87ebab27148fd96df06b80c0653b0`  
		Last Modified: Sat, 03 Apr 2021 06:48:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d4f55043ea94c3c4c7582c43b4a0aefeab551d8b423c8c6ca8a582a346526`  
		Last Modified: Sat, 03 Apr 2021 06:48:53 GMT  
		Size: 167.7 MB (167734337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460aaa8ea291f88d17f0f60340e88648366074aea3a5120b9b12ec2c7eefcc05`  
		Last Modified: Sat, 03 Apr 2021 06:48:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1658050c02486a8510fe506072336890bccdf5164d6c9bbac5688bec18773fd`  
		Last Modified: Sat, 03 Apr 2021 06:49:12 GMT  
		Size: 40.7 MB (40650845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6db4c1793003a6579a19d8b0d97bf2f1c23ed38d0e07ed39f34e8151b76a881`  
		Last Modified: Sat, 03 Apr 2021 06:49:01 GMT  
		Size: 281.4 KB (281385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4812b48766d2fb3e2fd98e48f4d37bd4a55bf445407ce68eb64cff5e9f7b68`  
		Last Modified: Sat, 03 Apr 2021 06:49:20 GMT  
		Size: 72.0 MB (71972623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44715f0482797f12571439c36a7779850eb41405628b40f0686be4862edc5401`  
		Last Modified: Sat, 03 Apr 2021 06:49:34 GMT  
		Size: 15.5 MB (15480070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
