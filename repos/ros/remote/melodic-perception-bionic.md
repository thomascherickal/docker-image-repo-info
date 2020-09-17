## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:0a8f208ac8fc46fa44745ce594fbe5006c1e399ad17ba7e980eb1ada5a1dc97b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:97228df74e8df583635aca2a871c99cb9ca8646a4824893420ec81f45ed3d867
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.2 MB (742221892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c91583c969c072fa04f54fb1cab32194840cae7d49cbd70d471d4b8978fa1f3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:45:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:00:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:00:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 20 Aug 2020 00:00:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 20 Aug 2020 00:00:54 GMT
ENV LANG=C.UTF-8
# Thu, 20 Aug 2020 00:00:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 20 Aug 2020 00:00:54 GMT
ENV ROS_DISTRO=melodic
# Thu, 20 Aug 2020 00:03:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:03:43 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 20 Aug 2020 00:03:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 20 Aug 2020 00:03:44 GMT
CMD ["bash"]
# Thu, 20 Aug 2020 00:04:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:04:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 20 Aug 2020 00:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaa5f3004b43b04fcf57d7f29efd6191edc973046054cb1590c6c134fd4064d`  
		Last Modified: Wed, 19 Aug 2020 23:06:36 GMT  
		Size: 838.2 KB (838225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a1a213ee0869dc0e68c035adc439944633af46f5812e47d6932677834acd6`  
		Last Modified: Thu, 20 Aug 2020 00:39:32 GMT  
		Size: 4.9 MB (4868690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f2e3eccb0c48240ffede5da52708cb96dacd1972e92214fc59d902972e09ad`  
		Last Modified: Thu, 20 Aug 2020 00:39:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299cf6e0456e79bfa74594d3e308221a0db2acd5a4647baab4bf80d84cbfbaa1`  
		Last Modified: Thu, 20 Aug 2020 00:39:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b82098ee61d3f8292fa778144a83c5f39fcfe250137de95b86360e944e1185`  
		Last Modified: Thu, 20 Aug 2020 00:40:25 GMT  
		Size: 259.3 MB (259254069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d598c779a1787b5d198f53223c81e6c14cde32b5a58c9e48e91c4f4c25a23627`  
		Last Modified: Thu, 20 Aug 2020 00:39:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf198ae82718018d06903cbacc4513a3c66f0c2d5e7220b1a0c813496d051be`  
		Last Modified: Thu, 20 Aug 2020 00:40:43 GMT  
		Size: 70.2 MB (70210460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c7260943ff92a69482df74de1fb4ed460f2f433d7fe311f656fb0bcd0bcb`  
		Last Modified: Thu, 20 Aug 2020 00:40:29 GMT  
		Size: 257.0 KB (257024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116d8e80d683b5e388eafd19fc30a30b4e47fa94e55d46fcc18c04e24d1b21bc`  
		Last Modified: Thu, 20 Aug 2020 00:40:48 GMT  
		Size: 75.0 MB (74984566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b36a6b82f8baf64c66e4fd8366db091bcc7070dd2a6f1948ed7056171c8dcc`  
		Last Modified: Thu, 20 Aug 2020 00:42:05 GMT  
		Size: 305.1 MB (305070556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:d552c079b155e25110c8c4045e7fae9add657e7d68f7c5ffcecf2bf6a12ea060
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.4 MB (645428682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15355f693c25fa1f740013cce765b9717c2556a28682222353f7b2f7a9eb6fab`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:28:20 GMT
ADD file:f239c31583452916dd5a653985cbb35d0acb5e97723cb8bcb089ab6dbc009543 in / 
# Wed, 16 Sep 2020 22:28:25 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:28:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:28:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:28:29 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:39:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:40:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:40:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Sep 2020 23:40:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Sep 2020 23:40:13 GMT
ENV LANG=C.UTF-8
# Wed, 16 Sep 2020 23:40:14 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Sep 2020 23:40:15 GMT
ENV ROS_DISTRO=melodic
# Wed, 16 Sep 2020 23:43:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:43:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 16 Sep 2020 23:43:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Sep 2020 23:43:43 GMT
CMD ["bash"]
# Wed, 16 Sep 2020 23:44:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:44:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Sep 2020 23:46:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:50:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46d8d5151783740c4f70c11c624110a72d6b7d8493331685c23eb44a666f962c`  
		Last Modified: Mon, 07 Sep 2020 15:50:39 GMT  
		Size: 22.3 MB (22279228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0959cf6d665929dbf2838b855f0075660add7f1c3faf5448a40700196e90b0`  
		Last Modified: Wed, 16 Sep 2020 22:30:31 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1764331539d248c00080a27564305167245f13addfdedad6507d51963b39257c`  
		Last Modified: Wed, 16 Sep 2020 22:30:31 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491b5d3c9f39553218974674ea250f3fb389092036ebb38a8af47267d5549cd1`  
		Last Modified: Thu, 17 Sep 2020 00:20:53 GMT  
		Size: 838.9 KB (838860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e462b6c5168c4d5a30db12ddc6821469b045aa66cc93b25d061dd70449178`  
		Last Modified: Thu, 17 Sep 2020 00:20:51 GMT  
		Size: 4.1 MB (4084274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84540db783e530a304a48855cbad8b87e5ff41c406ae1ddb38a585138a2174b`  
		Last Modified: Thu, 17 Sep 2020 00:20:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d9bb635f327fbdfd5b82228dda72aa3bc957d766fb7a7a3a75791c0a596325`  
		Last Modified: Thu, 17 Sep 2020 00:20:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2278b4de38bbdc7816ed5ca41513160c8a48e25d2fff61c40893f515cfd31346`  
		Last Modified: Thu, 17 Sep 2020 00:22:17 GMT  
		Size: 238.7 MB (238720345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910e1c2b76066ab6cf01e92b7e952bb55bdf622ea9912ced8ba4456fee45874`  
		Last Modified: Thu, 17 Sep 2020 00:20:50 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee94074e0ce759ead5a16b6d8e6ec6d00d9f59d00e7daaed4b1cbd6710930cf2`  
		Last Modified: Thu, 17 Sep 2020 00:22:40 GMT  
		Size: 54.7 MB (54684827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdcb2c0d1b17ebeb043a8f914decb500cee73de18243cce1a1c165fa4d4ea9d`  
		Last Modified: Thu, 17 Sep 2020 00:22:24 GMT  
		Size: 260.4 KB (260373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b152d4c4c5996b43a2640077a858f8a6133b64b99d142bd7a1961168cf60625`  
		Last Modified: Thu, 17 Sep 2020 00:22:47 GMT  
		Size: 64.7 MB (64747104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66cc15df2d27c0aa347d4e6150c102f4227d50de5ca30a42b62b23e6f871fd4`  
		Last Modified: Thu, 17 Sep 2020 00:24:31 GMT  
		Size: 259.8 MB (259810792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:65c47c1ea539dc663ae44ce705e846c2ef1c0a7cdcefe03a5adfa0579b712ed5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.2 MB (703203384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa132970864beb7caddb476427cf900d366208c3b1843996857d78c4d639cbc5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:29:47 GMT
ADD file:b8316fc82a2cf230ce4af7dcf02ec1d7e56b156cf610af8ed23b64509c77c799 in / 
# Wed, 19 Aug 2020 21:29:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:29:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:29:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:29:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:14:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:14:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:15:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:15:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 Aug 2020 23:15:03 GMT
ENV LANG=C.UTF-8
# Wed, 19 Aug 2020 23:15:04 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 Aug 2020 23:15:05 GMT
ENV ROS_DISTRO=melodic
# Wed, 19 Aug 2020 23:17:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:17:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 19 Aug 2020 23:17:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 23:17:52 GMT
CMD ["bash"]
# Wed, 19 Aug 2020 23:18:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:18:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 19 Aug 2020 23:20:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:237528ba509b2abcdba1ff1344bab27ad56235cdb3c1c131d3587f6fba4d92c9`  
		Last Modified: Sat, 08 Aug 2020 00:25:26 GMT  
		Size: 23.7 MB (23721798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b96f31d8b2bf3ce9eb4ac49e6c7411defa4057c1791f02f54c14f2de298ec`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 35.2 KB (35203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82b0e39008d2fa246a0dca4cfa5feb15db58591582a839bd69d5000aa2e96d`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ca375b8d34c9bc764ae24791184cba22510f0c002815b4f9766dd0463f5f5e`  
		Last Modified: Wed, 19 Aug 2020 21:32:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f6dffa388a5afeaeeec2de7d9fa800e94f1e7f1ad2274f59f7157286f86ec`  
		Last Modified: Thu, 20 Aug 2020 00:06:26 GMT  
		Size: 838.7 KB (838677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed841649442752ce9cf01dc1412c51934d12d590691361fb31a442d8793944`  
		Last Modified: Thu, 20 Aug 2020 00:06:21 GMT  
		Size: 4.5 MB (4451831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0e3e7bfbdedb57d66e251fe599446189354d4603eb3d458f1fedb2de4c72a8`  
		Last Modified: Thu, 20 Aug 2020 00:06:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5baf001431a2cb134fd89d60b9a68fa0b96080dc8d29a03089f22a49f4d9bfd`  
		Last Modified: Thu, 20 Aug 2020 00:06:16 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bfcca3905077b848174af84e561f71670359af5ab4020b3319a9c717b58e93`  
		Last Modified: Thu, 20 Aug 2020 00:08:22 GMT  
		Size: 252.2 MB (252197588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c56710b158762c9c68adce1ce8e74630d457eae838d541aa9028e9c0a96d1bd`  
		Last Modified: Thu, 20 Aug 2020 00:06:17 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a731e9acf679901cdaf8e15fe58dcbed5399efa25426787c0fab9b4e76f64b`  
		Last Modified: Thu, 20 Aug 2020 00:08:53 GMT  
		Size: 63.0 MB (63045898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d50da9773b39ecad201d028b05fd84a6c76011a19a242b99d4d5892fe8da4a`  
		Last Modified: Thu, 20 Aug 2020 00:08:33 GMT  
		Size: 257.1 KB (257072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a30a4ea0ee37c20d31f22231e630dd4bcb7423bde432569120343b7a77cf47`  
		Last Modified: Thu, 20 Aug 2020 00:09:18 GMT  
		Size: 67.2 MB (67223014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd835f0a8731d2857f57f54e2149a126f66fe15660a4817c2eb7556079218efd`  
		Last Modified: Thu, 20 Aug 2020 00:11:29 GMT  
		Size: 291.4 MB (291429424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
