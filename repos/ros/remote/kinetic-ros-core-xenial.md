## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:d20356614a760019d70434e2b7932e9c380ac560149deceb88b46e2ffccc4278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:4e79e4ac4f25b4b35c71bee4990516272c70629b6237107cd6682cf1d56b4a20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.0 MB (237031295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37814e1a9b51c00a65f407329ef4ace680d86cb4aff7cc311c2643bed5b4f324`
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

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:631382e4269308de7282ec0a7d4c596e08659072e6409f3c252a86271ddc8463
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212547342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa63fe9fbc1927b9f0f68c0a651875d8c78fa2963bfab40b0d203d6ca7b5028`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 18:17:14 GMT
ADD file:5c0d6a48e839c912491edae36f7465b9efe445d4a5ee58861fee1ccd424890ec in / 
# Fri, 23 Oct 2020 18:17:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:17:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:17:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:17:22 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:54:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:54:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 18:54:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 23 Oct 2020 18:54:28 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 18:54:29 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 18:54:29 GMT
ENV ROS_DISTRO=kinetic
# Fri, 23 Oct 2020 18:56:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:56:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 23 Oct 2020 18:56:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 18:56:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:183a558dd6745131430d26859b5c0b308384044df34cc35f69c406432c022d3a`  
		Last Modified: Mon, 19 Oct 2020 17:04:41 GMT  
		Size: 39.9 MB (39897338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c9cb164a2e061f22d5b157a0e96dcd278984851436ba61b9eeafd17cd0a8e4`  
		Last Modified: Fri, 23 Oct 2020 18:18:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3963d7d3f6c0b3ca836f488586277a576d3477f7976e185bbbc4b79fea203`  
		Last Modified: Fri, 23 Oct 2020 18:18:14 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da982e99c6f88739b993432f872f7b916b7f2c3d185cadf69c4ebbf511964e2`  
		Last Modified: Fri, 23 Oct 2020 18:18:14 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf93f7cf1c717a7e93b88e644ef1c651835d4214ad288e5a4b8e409355e9a6`  
		Last Modified: Fri, 23 Oct 2020 19:15:27 GMT  
		Size: 4.6 MB (4614846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9133d92cbd0a86346bbabc16b7efeef8edcf85420898da7ebbab948e3a312fda`  
		Last Modified: Fri, 23 Oct 2020 19:15:26 GMT  
		Size: 14.7 KB (14744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed55684850ac54be387a7869f7aa3ec3f663d7db8097700ef42817c7524c1a2b`  
		Last Modified: Fri, 23 Oct 2020 19:15:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65972f4a630f6d2690c798e849ad315dc4f536ee2718212a6fa6da3d054ce465`  
		Last Modified: Fri, 23 Oct 2020 19:16:28 GMT  
		Size: 168.0 MB (168018463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce33d191d74030c32fcfceb9ce1b0fe70b43d34510fafd9ee77220686d35c94`  
		Last Modified: Fri, 23 Oct 2020 19:15:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b6acf358cb32657808011049529e39e81ee6e2d34385271c223632b887981927
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.9 MB (220927974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aee0199fdc983246f6bc80796d87d39779345ab0c8330bd40c07a94d9a8f4783`
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
