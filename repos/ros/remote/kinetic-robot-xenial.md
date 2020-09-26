## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:1e9b93c17272b9dc0b7f479ce939786d148cf65173c5c1d96d9a8c69b22a8a5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:cc051ea3ea6ae3e68dc016dcf6020f7222e951629d1e88a75a2919ba6054dcd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.6 MB (379617668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4777130028d84294a8365ea99f95dc8397acf0a509e3e343d119f299522792`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:36:27 GMT
ADD file:23a55d7e93b396e490b6d0893137e5c13e3e0a234e0feaea8b1cfd4079fb1882 in / 
# Fri, 25 Sep 2020 22:36:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:36:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 22:36:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:36:29 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:28:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:28:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 01:28:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 01:28:19 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 01:28:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 01:28:20 GMT
ENV ROS_DISTRO=kinetic
# Sat, 26 Sep 2020 01:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:30:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 26 Sep 2020 01:30:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 01:30:27 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 01:31:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:31:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 01:32:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:32:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f53fa4d2cf0e29c6a522433e0ac71a7ce0fdab158481052b2198b5518b83248`  
		Last Modified: Thu, 17 Sep 2020 13:19:58 GMT  
		Size: 44.5 MB (44517215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af7c939e38e8e3160fbbdcc26a32669529b962c79f7337df0a26bf0e9a76d59`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903d0ffd64f6ca1355d2b2df702fc674f5663981dfd100fe4588fb390dd3382c`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04feeed388b71fdca5cc3bce619d65a34f8a1a3e5b0ef03f8392d499970818eb`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5d9e557739a877f9ba447fbf56cb1ada15ab6fd91ed67b831e953b7cab336`  
		Last Modified: Sat, 26 Sep 2020 02:11:54 GMT  
		Size: 5.4 MB (5362191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cf7dc8e9dd4a0f511731b11ec56c3e67d306976b0a13869b1cef600d5508b0`  
		Last Modified: Sat, 26 Sep 2020 02:11:53 GMT  
		Size: 14.7 KB (14742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce364a0df57530f80445d16045ee42fcb267f40d7517f51e075aae0a2724e7d`  
		Last Modified: Sat, 26 Sep 2020 02:11:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a5063cb92e828b306a106c6ce6abbebf89dcf586f2ff5f50446e4f038ccb58`  
		Last Modified: Sat, 26 Sep 2020 02:12:38 GMT  
		Size: 187.1 MB (187135180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d78c4f840cf0d2c146db6cb0435eff918c12d1d1d3b0efb52b6ab27a3ec069`  
		Last Modified: Sat, 26 Sep 2020 02:11:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cea0f40936bbd3196c1d22c28bc138ac5f9900305ff30a49e6d1420e32a142`  
		Last Modified: Sat, 26 Sep 2020 02:12:54 GMT  
		Size: 57.2 MB (57240396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d506e21ad5f22cc1a8082965c2b42b1fc2deb801ff5ec8eeaf479b3c29bf318b`  
		Last Modified: Sat, 26 Sep 2020 02:12:42 GMT  
		Size: 265.2 KB (265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d07ab587f259253d7d92193e89c8e12211b32d53be3025334e1ebdeea09c1aa`  
		Last Modified: Sat, 26 Sep 2020 02:12:58 GMT  
		Size: 63.6 MB (63576594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e5d98c1847182232bf60baab593908c97d94b7053c8bc318a3dbe78bdd5d1`  
		Last Modified: Sat, 26 Sep 2020 02:13:08 GMT  
		Size: 21.5 MB (21504208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:bc0e8039fd70a2f9b71350fa8d66eca814ca83815cfd2a3f60d21936dbdd1e51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330646900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4696a5ec219362719ed2bb314accaf4685ae7d209a1a625f3c3b80263151cac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:06:05 GMT
ADD file:4d80806eb22c42514472851b887a765784dc20eeef88bde0c3caeb9291888791 in / 
# Fri, 25 Sep 2020 23:06:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:06:12 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:06:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:06:15 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:40:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:40:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 25 Sep 2020 23:40:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 25 Sep 2020 23:40:56 GMT
ENV LANG=C.UTF-8
# Fri, 25 Sep 2020 23:40:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 25 Sep 2020 23:40:59 GMT
ENV ROS_DISTRO=kinetic
# Fri, 25 Sep 2020 23:43:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:43:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 25 Sep 2020 23:43:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 Sep 2020 23:43:52 GMT
CMD ["bash"]
# Fri, 25 Sep 2020 23:44:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:44:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 25 Sep 2020 23:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:46:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:485f48bc272eae39f18c1a9176e66e8b966dbb4a3e508b91d5a3033dd0daa471`  
		Last Modified: Mon, 21 Sep 2020 16:00:14 GMT  
		Size: 39.1 MB (39081505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd10a909e2213bb0572a2db9009e10cda02123be17e446b22c9d39409f36d735`  
		Last Modified: Fri, 25 Sep 2020 23:07:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29722351f2ca14bda92f7440d88e522ec18a053f73a29573491c3e1cba0f3e7`  
		Last Modified: Fri, 25 Sep 2020 23:07:22 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bd49b76010ec54442b6a768989972c3299f6696b6598201b6b86ac74488c12`  
		Last Modified: Fri, 25 Sep 2020 23:07:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246607ca1d96be44d2d1afa1908cdb57cba6b7f9eb4285fe71a2aec0ae1de739`  
		Last Modified: Sat, 26 Sep 2020 00:38:39 GMT  
		Size: 4.6 MB (4614837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d022e13e82a1d135a6d0227cc0023e809128f53181ce096dba805cdb5d1653`  
		Last Modified: Sat, 26 Sep 2020 00:38:37 GMT  
		Size: 14.7 KB (14740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c01a860f54c4af962c27c3f1cc76d41a90defa98cf25ae27300070fbe14ad`  
		Last Modified: Sat, 26 Sep 2020 00:38:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d659582a0efac9144fa7d6cdd2f7a6f55df501632bf4728f5c3f20bd592d018`  
		Last Modified: Sat, 26 Sep 2020 00:40:31 GMT  
		Size: 168.0 MB (168016908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34992948fe045770dc27db2a4adb0e902098d1e7dd8922591b48f5a6f9681ac9`  
		Last Modified: Sat, 26 Sep 2020 00:38:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5713c51efef090e4158ae3f4fabc2ddc6c9d4544abe83a7423763fce2b33cb50`  
		Last Modified: Sat, 26 Sep 2020 00:40:52 GMT  
		Size: 42.9 MB (42892175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b3e5b062a2dbe5079a39f49ef458304fbdf1387b1bae9bcbb153a2a8a3a87`  
		Last Modified: Sat, 26 Sep 2020 00:40:39 GMT  
		Size: 265.1 KB (265085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6892cdc79858feb9ae254e4f145ba9829cbd9ed835680a1b06b4b449cbc2c333`  
		Last Modified: Sat, 26 Sep 2020 00:40:59 GMT  
		Size: 55.5 MB (55502838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876afe946b4834681cbd8163c18e7140d96170896168a63e254db2f4fc06d0a1`  
		Last Modified: Sat, 26 Sep 2020 00:41:25 GMT  
		Size: 20.3 MB (20256862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:77894bf32924e3c17b60587e9c8e4d916038fc68e0884e6f12196da59b5b0828
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.0 MB (344961718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df632783e75756f31b82dec225f36768ad01739985b88109de4cd73c73adf32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:48:52 GMT
ADD file:5ad8fe01e35cc6efe923d7698aaa261cdb15f4f4ae01009d04d2a1ddadc1d5b2 in / 
# Fri, 25 Sep 2020 22:48:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 22:48:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:49:00 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:06:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:06:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:06:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:06:07 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 00:06:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 00:06:10 GMT
ENV ROS_DISTRO=kinetic
# Sat, 26 Sep 2020 00:08:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:08:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 26 Sep 2020 00:08:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:08:36 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:09:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:10:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:11:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:511338b9646fd6cab2c278e174281c8d444bef1a2846348b1e0687ece0450d3c`  
		Last Modified: Wed, 16 Sep 2020 16:25:23 GMT  
		Size: 40.1 MB (40099025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b39b0ff65d844135c15ee00abc2dec8e0a964a0f626097ba95ee4c2fa0a19ed`  
		Last Modified: Fri, 25 Sep 2020 22:50:25 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a1f7ba18a1a2b6ece87fc83510da11658ea364ee85e16467c0ca7cfadb52d7`  
		Last Modified: Fri, 25 Sep 2020 22:50:26 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caa76f7dac8b4a5afba79f1582f3546a987a066f79adb97b5dfa25b0f72989a`  
		Last Modified: Fri, 25 Sep 2020 22:50:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aae363fcab0e9c7a4abd4bed533df0f9de2c2ef8ddc2202f62dc672cd49fb6`  
		Last Modified: Sat, 26 Sep 2020 01:15:51 GMT  
		Size: 4.8 MB (4819812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d8be871ebee263ac21629cfd32299af5a2d1ba2be0cb80afb022170bc02cc`  
		Last Modified: Sat, 26 Sep 2020 01:15:50 GMT  
		Size: 14.7 KB (14743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7823676f1e566f1f924ab62c452dbd31f2284b372cebf93604adc57818b8639`  
		Last Modified: Sat, 26 Sep 2020 01:15:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbf1ffdf3a6ab5fc0092401c9e4444bdefd1472567f77d23882946cfdea6088`  
		Last Modified: Sat, 26 Sep 2020 01:17:58 GMT  
		Size: 176.0 MB (175992481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e609819121d940fab843b401b583d9dbc1e813240bd774cc944515aacc6f42fb`  
		Last Modified: Sat, 26 Sep 2020 01:15:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b720bcc0cc4581da5313cae71a9167bbe2b80364cdf6e0b4dec21ea6e092c48b`  
		Last Modified: Sat, 26 Sep 2020 01:18:20 GMT  
		Size: 46.0 MB (45952449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d33c52b8b8649ddd510b8b49f5fb98d166b83e195642181f9fb683dd6574d6`  
		Last Modified: Sat, 26 Sep 2020 01:18:06 GMT  
		Size: 265.2 KB (265219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d895c68637f71f191a6537ebadda8ac41baa47ed34802413d05633afcdb18077`  
		Last Modified: Sat, 26 Sep 2020 01:18:29 GMT  
		Size: 57.3 MB (57298165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4678a57a17fa071b797854f8691b70140d4103b36378b3ea39e06a44ff4703c1`  
		Last Modified: Sat, 26 Sep 2020 01:18:47 GMT  
		Size: 20.5 MB (20517911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
