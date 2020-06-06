## `ros:latest`

```console
$ docker pull ros@sha256:2bfeaf8e7f448432a0b45795d1b9b0c6f9617bcfd032a3e7c50bd73759548373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:4a07ce5bed8619a8b1872f9c123e327751668cd7b77ebc765038e464b14e6ef4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.5 MB (435456984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91bc7caeebc64e222055f8e08ce3c8a626ec1b8b6d5e7378b4de32477ef5ccfc`
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
# Wed, 27 May 2020 00:29:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 May 2020 00:29:36 GMT
ENV LANG=C.UTF-8
# Wed, 27 May 2020 00:29:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 May 2020 00:29:36 GMT
ENV ROS_DISTRO=melodic
# Wed, 27 May 2020 00:32:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:32:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 May 2020 00:32:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 May 2020 00:32:53 GMT
CMD ["bash"]
# Wed, 27 May 2020 00:33:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:33:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 27 May 2020 00:34:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:dea62d652c77bd34ca26f69339248661821c83a5dce8d31845128e620eae5a60`  
		Last Modified: Wed, 27 May 2020 00:53:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f798296ec2caa37a3146f3c49d4a6fea76f0e80b4c3ad1e2d3a0733ea405da4`  
		Last Modified: Wed, 27 May 2020 00:54:43 GMT  
		Size: 259.2 MB (259241668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87b1a5103eec8d6562a9bd1248218a06876ab6169d32111a31fd7454a264122`  
		Last Modified: Wed, 27 May 2020 00:53:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6887a4344fda2ee2597752bcf759aa0cf943b84026c65f86a627dab3c36718a9`  
		Last Modified: Wed, 27 May 2020 00:55:03 GMT  
		Size: 70.2 MB (70209920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d491308ce011d7853bf7f0ce0db5c40457b6f745420934cb684d2f8bd4217372`  
		Last Modified: Wed, 27 May 2020 00:54:48 GMT  
		Size: 248.1 KB (248104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7f7e1d40461ce3e72e418080d7379f0945d29b0cf2536ac3c3ceef8a5b4baa`  
		Last Modified: Wed, 27 May 2020 00:55:07 GMT  
		Size: 73.3 MB (73324470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6576db63ee4fc6ab4bd5af2a8685cf3ad454400e9fabb4afadec2d323014f589
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207750836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e190bb503c0b3920813f8588b748a9515422efe57adb78966278a951b164daf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:18:16 GMT
ADD file:e9947aff2dfa8f220d4b25dc0770aff8d9ffc08482e52f54833f39e1c3ec08bf in / 
# Fri, 24 Apr 2020 00:18:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:18:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:18:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:18:29 GMT
CMD ["/bin/bash"]
# Wed, 27 May 2020 01:42:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:43:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:43:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 06 Jun 2020 00:42:37 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 06 Jun 2020 00:42:38 GMT
ENV LANG=C.UTF-8
# Sat, 06 Jun 2020 00:42:39 GMT
ENV LC_ALL=C.UTF-8
# Sat, 06 Jun 2020 00:42:40 GMT
ENV ROS_DISTRO=foxy
# Sat, 06 Jun 2020 00:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 00:44:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 06 Jun 2020 00:44:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 06 Jun 2020 00:44:38 GMT
CMD ["bash"]
# Sat, 06 Jun 2020 00:45:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 00:45:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 06 Jun 2020 00:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 06 Jun 2020 00:46:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c2d76ba33f8d52087147ce28d8f03c08f69677591e3e10db810bf76a6e09427`  
		Last Modified: Fri, 24 Apr 2020 00:22:00 GMT  
		Size: 27.2 MB (27158644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d4cfc71d3821474946021fdbf241a74992a84c6269c3e9a052ce7fc56cece`  
		Last Modified: Fri, 24 Apr 2020 00:21:52 GMT  
		Size: 32.3 KB (32326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63063bfe137200b3c8d1ee8d819124352c20ee8c189a0388f461ec66bb759310`  
		Last Modified: Fri, 24 Apr 2020 00:21:53 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38385900086ffa7d7cb9c3bbeabaf2176d7d7958ebf0736d2a01773a830201ee`  
		Last Modified: Fri, 24 Apr 2020 00:21:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee47658e5a2b6951b5c8f1df079e5f94fa5babfcb132843f7e89a21a531555f5`  
		Last Modified: Wed, 27 May 2020 02:09:35 GMT  
		Size: 1.2 MB (1175483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b7e5841799d26c7c96bfbade1ef6d8be3e67adbbc8402a26e6a6cf491a849`  
		Last Modified: Wed, 27 May 2020 02:09:35 GMT  
		Size: 5.5 MB (5515489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8079fbc9cd40b2782019694e3fdfea45d641b7cd63c3e41e193edc9581c050ee`  
		Last Modified: Wed, 27 May 2020 02:09:33 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3ec18d9d03c6ef880ba9e4caecbbfd50402843b4d260e38bf7d308700a606`  
		Last Modified: Sat, 06 Jun 2020 00:46:59 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526f25ed5278e2e7a7fde79b21330117bd4b9e32b6b5232ae881703bdcd287aa`  
		Last Modified: Sat, 06 Jun 2020 00:47:30 GMT  
		Size: 103.5 MB (103476592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc209a31a5ea7c241b1c1de254415f9a26b41a629573e40f2deb838c76a0571`  
		Last Modified: Sat, 06 Jun 2020 00:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc422b8040cae43e2cffe00a313538b1cb4403997bb7d1d04d93dd6428032d37`  
		Last Modified: Sat, 06 Jun 2020 00:47:54 GMT  
		Size: 60.9 MB (60920850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c19a97d639dd8b2ffa7aab57eb52443168bccc100f9d52ca0fec80a6bdcab3`  
		Last Modified: Sat, 06 Jun 2020 00:47:38 GMT  
		Size: 178.1 KB (178053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ec65a6dc3c1e370aff3a74854a2b8125875dfeca9bb569a2b4fb6e068fde1`  
		Last Modified: Sat, 06 Jun 2020 00:47:38 GMT  
		Size: 2.0 KB (2016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa53f0e6cd1fca763eb9c735bc6aa6e64c8b8688e32422adc1eedc51b6fc8bb`  
		Last Modified: Sat, 06 Jun 2020 00:47:41 GMT  
		Size: 9.3 MB (9288504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
