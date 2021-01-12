## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:f7753073d1c21603d3021a13fc46f86012ac5ee9480f10280442fcce1ee2c23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:537f792e5d003317d24f5645aff9d2021d209871bd1507afd4229bd65dbb5b0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.7 MB (334735301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3b7dadb6f5874e89eaccf26bd1fbb107f92c085fe797a8a69f2bfffa6069be1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:07:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:59:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:59:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 26 Nov 2020 02:19:59 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 26 Nov 2020 02:20:00 GMT
ENV LANG=C.UTF-8
# Thu, 26 Nov 2020 02:20:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 26 Nov 2020 02:23:04 GMT
ENV ROS_DISTRO=rolling
# Thu, 26 Nov 2020 02:23:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:23:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 26 Nov 2020 02:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 26 Nov 2020 02:23:55 GMT
CMD ["bash"]
# Thu, 26 Nov 2020 02:24:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:24:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 26 Nov 2020 02:24:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 26 Nov 2020 02:24:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:24:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 26 Nov 2020 02:24:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 26 Nov 2020 02:24:57 GMT
ENV ROS1_DISTRO=noetic
# Thu, 26 Nov 2020 02:24:57 GMT
ENV ROS2_DISTRO=rolling
# Wed, 02 Dec 2020 19:31:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:17:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.0-1*     ros-rolling-demo-nodes-cpp=0.11.0-1*     ros-rolling-demo-nodes-py=0.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:17:58 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5df4314d5099f1cf2100a5313a0658ed554a2983ba59b623b5bad8c4809e05`  
		Last Modified: Thu, 26 Nov 2020 02:31:32 GMT  
		Size: 1.2 MB (1178529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c14ddc5480deadf9144c474a609532b85769b3254ed91b971659b90177719f`  
		Last Modified: Thu, 26 Nov 2020 02:31:32 GMT  
		Size: 5.5 MB (5547277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0070f07bf5a4e96efca137c61d59aaadf64010bc606c054d868f3afa6e44a981`  
		Last Modified: Thu, 26 Nov 2020 02:31:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9effa899cb9a89f581ee93ba079029c694a6fb10175cfeb3309ebc4551872a`  
		Last Modified: Thu, 26 Nov 2020 02:37:49 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279675193622226863d2accf21f93581d754d3cc767cf826e516b87dc3db5e3b`  
		Last Modified: Thu, 26 Nov 2020 02:39:51 GMT  
		Size: 119.6 MB (119589291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078e688a9d7470ed7945fd897dd8706a44e54faa117af3cddab0b75ce4ed9e2`  
		Last Modified: Thu, 26 Nov 2020 02:39:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f69afe775a00eb582006e78d5292f9a00125eea9eaadeacea3629bf869bd615`  
		Last Modified: Thu, 26 Nov 2020 02:40:10 GMT  
		Size: 66.6 MB (66588090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcf884fe79efaad0e13cb4249d690c0e4ca003dd43375c7681945a64f83bd7c`  
		Last Modified: Thu, 26 Nov 2020 02:39:56 GMT  
		Size: 191.9 KB (191864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e13fa34c164e85d3585644067165e6f28003f00a4abbeb89c68a779387d78da`  
		Last Modified: Thu, 26 Nov 2020 02:39:55 GMT  
		Size: 2.0 KB (1971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06e9b59af3f86339cf1866af69ee107bec19189c301fab2007da6a7eceb74d1`  
		Last Modified: Thu, 26 Nov 2020 02:39:59 GMT  
		Size: 10.5 MB (10476192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81b55a9a3cd3fc4a7a2118626f47b2dcc057cf111ef5a5f9fa0f798f0a54bb`  
		Last Modified: Thu, 26 Nov 2020 02:40:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5d40c8940df51e23f4ca90f51160421dbe8d2812a011b72c1565a9269f848e`  
		Last Modified: Thu, 26 Nov 2020 02:40:16 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb259285a832ef5d4208863a89ddcd48b63ce4069b29ee253fe756cadf14d27`  
		Last Modified: Wed, 02 Dec 2020 19:33:52 GMT  
		Size: 76.1 MB (76088688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e791116ccb1c8f5bf341c797beba5228bc99c41f13d6a6777f484e6ae72ef697`  
		Last Modified: Tue, 12 Jan 2021 01:29:20 GMT  
		Size: 26.5 MB (26506655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b67f436ea826b386be55dc5c2b2fd7cdd6cf4c4237402f8365dfdb8a9873677`  
		Last Modified: Tue, 12 Jan 2021 01:29:11 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87eff54e79af0ccf3aed9daf5db726445233b2e31c6db1f603320785bfd90955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.9 MB (307927151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd23a14eede313e07e3e9e61265802f6609262fa446166abb02030ce3618c87`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:43:12 GMT
ADD file:a9ede6466d698f7a9f018b5121f755f98a7322ba320e16ad207aaf3819ea8bc2 in / 
# Wed, 25 Nov 2020 22:43:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:43:17 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:09:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:09:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:09:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 26 Nov 2020 00:47:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 26 Nov 2020 00:47:48 GMT
ENV LANG=C.UTF-8
# Thu, 26 Nov 2020 00:47:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 26 Nov 2020 00:55:37 GMT
ENV ROS_DISTRO=rolling
# Thu, 26 Nov 2020 00:57:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:57:46 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 26 Nov 2020 00:57:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 26 Nov 2020 00:57:51 GMT
CMD ["bash"]
# Thu, 26 Nov 2020 00:59:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:59:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 26 Nov 2020 00:59:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 26 Nov 2020 00:59:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:00:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 26 Nov 2020 01:00:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 26 Nov 2020 01:00:16 GMT
ENV ROS1_DISTRO=noetic
# Thu, 26 Nov 2020 01:00:18 GMT
ENV ROS2_DISTRO=rolling
# Wed, 02 Dec 2020 19:07:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jan 2021 23:53:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.0-1*     ros-rolling-demo-nodes-cpp=0.11.0-1*     ros-rolling-demo-nodes-py=0.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jan 2021 23:53:35 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a970164f39c1a46f71b3615bc9d5b6710832766b530d9179db8e36563f705abb`  
		Last Modified: Fri, 06 Nov 2020 16:25:39 GMT  
		Size: 27.2 MB (27168047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c66f1fb5a2d6587841797a3b0d4c2d0fd0b7ccd867e55a1314cee2e90ad47d`  
		Last Modified: Wed, 25 Nov 2020 22:44:54 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94362ba2c285844f83a1b1e2dac5217b0426427f8bb809af534b5f4d751e298c`  
		Last Modified: Wed, 25 Nov 2020 22:44:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3b8010f6524f19985954a3e2167cad0144281b8110f953aaba2cee0c1ffc86`  
		Last Modified: Thu, 26 Nov 2020 01:10:26 GMT  
		Size: 1.2 MB (1179446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dd5cea3e60bcb0505d291a9eef2e4731c326a5c88016c41a808bfa86a10011`  
		Last Modified: Thu, 26 Nov 2020 01:10:26 GMT  
		Size: 5.5 MB (5513913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8060ab4d8e27c250b390e230c79dcd8b785946fa7657a84723b397785b1475da`  
		Last Modified: Thu, 26 Nov 2020 01:10:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bb2de6dad66673754498d37d5169628357c503c803c2ea64a866df657d25cf`  
		Last Modified: Thu, 26 Nov 2020 01:18:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6409cee42415a7bfd295638de227f112e8b759d4c7630dd8420a5b78e900c2`  
		Last Modified: Thu, 26 Nov 2020 01:20:31 GMT  
		Size: 103.8 MB (103796169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4867891e77146128d51b092a191f0c9b3f17e77f451cfa513718f703acd815ed`  
		Last Modified: Thu, 26 Nov 2020 01:20:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f0937401a5b26bef3ea3c57bc09ad94a807a0d80b2d41571c4b72455371d9`  
		Last Modified: Thu, 26 Nov 2020 01:20:54 GMT  
		Size: 61.0 MB (60961082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855bc515eef22b45b78de2c8e291fba0a87f1f5b07438d427f9d635dc4feb41`  
		Last Modified: Thu, 26 Nov 2020 01:20:39 GMT  
		Size: 191.9 KB (191919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2e66306ed700a6db665ff6a9b49eb922811b4691b60c6f01e1d9f620a5d377`  
		Last Modified: Thu, 26 Nov 2020 01:20:39 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348c848fa48ebc90031243a2f7d4403923ecd55c1a81096e229854998c072925`  
		Last Modified: Thu, 26 Nov 2020 01:20:42 GMT  
		Size: 9.5 MB (9488486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e1faa7ad2d5174cdd83b82087c18e1cda560ceeb8e81f3d630e64061e1cd54`  
		Last Modified: Thu, 26 Nov 2020 01:21:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a74fee6df57aa031478bfe9c871e9baf5a96d31ff95e913be8dda01ba4f857`  
		Last Modified: Thu, 26 Nov 2020 01:21:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc9420a79cb3e212d81a146214eb9e4dee507dc5ca8b27dbc709fa84f213a4`  
		Last Modified: Wed, 02 Dec 2020 19:10:59 GMT  
		Size: 76.1 MB (76141532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad74a92b88a29355a592f9ed9b7a92b34e126fd01b6592aae9d98042bbac5064`  
		Last Modified: Mon, 11 Jan 2021 23:56:02 GMT  
		Size: 23.5 MB (23481001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c5b290fd5546ba6d6bbbb7c80065edc7f86741e949a5022f0e4293a76978`  
		Last Modified: Mon, 11 Jan 2021 23:55:57 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
