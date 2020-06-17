## `ros:noetic-robot`

```console
$ docker pull ros@sha256:6e0ee23a1d7bdabcd1efd09eaf8af9c18eab567103676558d1f6628c461d184b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:f0b6f77e07940f8dac6781be28a3566e09f9e2da5df161609b17a9ca9067ad29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.4 MB (350369555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73dd0260a6d4d93ce7af105fc27b025bd4d8dc3c5200bf950bfc72ae140fde19`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:53 GMT
ADD file:b2342c7e6665d5ff3850d4f04e2521d1851eb2054f9a8d56fcf4e7c314b9f20e in / 
# Wed, 17 Jun 2020 01:20:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:56 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:23:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:37:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:37:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 05:37:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 05:37:36 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 05:37:37 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 05:37:37 GMT
ENV ROS_DISTRO=noetic
# Wed, 17 Jun 2020 05:39:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:39:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 05:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 05:39:42 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 05:40:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:40:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 05:41:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:42:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4a2a29f9ba48efd3d2075f395538b2eec56fb1bedfb7aecf5e54174446f9e2a`  
		Last Modified: Sat, 06 Jun 2020 15:19:59 GMT  
		Size: 28.6 MB (28556492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127c9761dcbaa288abc58fc56437c2f2ffbe611b9f7f30e0b5b43cd348bb2094`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 32.3 KB (32317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bf203e905463e64d89b14509aafa983fb8baf7c1931fe0a65652aeb6c838f`  
		Last Modified: Wed, 17 Jun 2020 01:22:01 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039240d2e0b4bcb42ccbce75bc54570e471ad81457478de35fbeef63536e9c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7dc0f500f30d268233b31f578ef235db8b98a2d1fba104ad604913847559df`  
		Last Modified: Wed, 17 Jun 2020 03:35:17 GMT  
		Size: 1.2 MB (1175466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84236ce676e3f1e78e38af3f125fbde6ca6c98b9f402fe3aea636df839e22ac`  
		Last Modified: Wed, 17 Jun 2020 06:05:46 GMT  
		Size: 5.5 MB (5549138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38529422ac2087523db3e5fba2c5d2cf139c13c59c865328241c9fa5e6ca63f6`  
		Last Modified: Wed, 17 Jun 2020 06:05:45 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7795c53dc42446f5316ccc12df4188839d9c3a14de9ef06fc60930837499b1`  
		Last Modified: Wed, 17 Jun 2020 06:05:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71414345f65e7419e820225a8d89cb64aa6b2847a93696418e68ca693bae6d8e`  
		Last Modified: Wed, 17 Jun 2020 06:06:29 GMT  
		Size: 173.0 MB (173040629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be317a0c7e8482c417ffc868c1f38f8b5eed417e908020aa421f9dc073f3a82`  
		Last Modified: Wed, 17 Jun 2020 06:05:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b7adaaac556e49f8139b1f7c7ba8b4d0134fdbf08658a3b175a1c279b8181b`  
		Last Modified: Wed, 17 Jun 2020 06:06:44 GMT  
		Size: 46.4 MB (46376367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c2b56e60447fbba4074fc859e9f186bf855560a6a81d5a886e5a69810fd4a`  
		Last Modified: Wed, 17 Jun 2020 06:06:35 GMT  
		Size: 202.2 KB (202155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b8090b9b215f87e3dffa6143193f6593181eda19ce98ecb92e87f6c59b6f4`  
		Last Modified: Wed, 17 Jun 2020 06:06:51 GMT  
		Size: 79.6 MB (79588961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29cb2b572faa11ba28f07dc4512ae5a98678c1ea8902c9e1eef1b9cbd8211d66`  
		Last Modified: Wed, 17 Jun 2020 06:07:01 GMT  
		Size: 15.8 MB (15845194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ae1457de01d801227eb8ba31eb8b5193ebe7e47115a680af6ccd3045afe0e181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329637881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2c847e18a75cafaa7666ddc4334af549ca634a46e935d4157e910ae89a4fca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:43:22 GMT
ADD file:6d1bd041dcbfb2d51c871c8eb820202f5597b37ac4e4b94ce976fbc157619c8e in / 
# Wed, 17 Jun 2020 01:43:25 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:43:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:43:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:43:33 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:58:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:58:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:58:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 03:58:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:58:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:58:16 GMT
ENV ROS_DISTRO=noetic
# Wed, 17 Jun 2020 04:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:00:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 04:00:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 04:00:18 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 04:00:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:01:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 04:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:02:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63de6a4b0fc89f1aa36d95a840e6729cca22d2abaa887bfaf634c40ad4560ed4`  
		Last Modified: Sun, 07 Jun 2020 08:26:19 GMT  
		Size: 27.2 MB (27159755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243514e240f4c2654743395ffa5aed01b5eaf985f0118cdb2089629e0e9747d8`  
		Last Modified: Wed, 17 Jun 2020 01:45:14 GMT  
		Size: 32.3 KB (32336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ba51c40fb5f743fb4a4050b63644e7727c21a1cffba4c4767ac41118ac6d3`  
		Last Modified: Wed, 17 Jun 2020 01:45:14 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684e0fb606a03cddd5fc30fb6aee6055e851951eff13e4859295a3097063bba7`  
		Last Modified: Wed, 17 Jun 2020 01:45:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7becc6ba0698cca4766101c1e07007231a2bbad3952ec0c01c4706b5dc09c`  
		Last Modified: Wed, 17 Jun 2020 04:40:14 GMT  
		Size: 1.2 MB (1175791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ab96636dc90f9fea2726c2bf53a0f70a76853a496b08e0f3420bb95ef55dea`  
		Last Modified: Wed, 17 Jun 2020 04:40:13 GMT  
		Size: 5.5 MB (5516600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da0b15f3c3835f213d1d6997096f6e6d9cf7b0bcd50604bcca3b1575907e09`  
		Last Modified: Wed, 17 Jun 2020 04:40:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b693847db75019ee2418a13d50ba5387b6a22fc763809dee7e66b1943ec92b9`  
		Last Modified: Wed, 17 Jun 2020 04:40:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91ea96a6ecbd7cd95d44152f610e8d554391d3267954942d549f8453a3c9161`  
		Last Modified: Wed, 17 Jun 2020 04:41:06 GMT  
		Size: 167.5 MB (167521995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a6ac536ca4a8d0a50cfb68401069edb5b681ae21d3d5d6c227fcb7e4a349a9`  
		Last Modified: Wed, 17 Jun 2020 04:40:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47412ee8f5f5b92ad85e542b0b1fd8aa9c3c521d3ea2f80c4aad67dbc581970d`  
		Last Modified: Wed, 17 Jun 2020 04:41:29 GMT  
		Size: 40.6 MB (40626722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881aaea0b479e882592bbabdcd383c372ffd7412804dc3f636e3a8335f829634`  
		Last Modified: Wed, 17 Jun 2020 04:41:18 GMT  
		Size: 202.2 KB (202214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2e76783ef01ac8f5beb06b488d9d0004a47a65a4aae0395e371bec200170d1`  
		Last Modified: Wed, 17 Jun 2020 04:41:38 GMT  
		Size: 72.0 MB (71968226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260ade2920471bfeb37bc00bee498ac507158db76f12eee19e49e9f96e037b69`  
		Last Modified: Wed, 17 Jun 2020 04:41:50 GMT  
		Size: 15.4 MB (15431362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
