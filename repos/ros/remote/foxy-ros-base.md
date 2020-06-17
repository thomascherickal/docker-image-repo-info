## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:0df1623d137eb9030d5b7bfd230b443ab1799512ff76093f26bb5baa4e7ad81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:ec5a228211c2ad8633e2d2d06276a07b0e120ab9409f9fa7d8308b43f0ddb364
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231594739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37ad8befce7a15c5fb3973a5f5c7a3ad74df9266f9f0383d2afb408512baaec`
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
# Wed, 17 Jun 2020 05:57:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 05:57:18 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 05:57:18 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 05:57:18 GMT
ENV ROS_DISTRO=foxy
# Wed, 17 Jun 2020 05:58:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:58:16 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 05:58:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 05:58:16 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 05:58:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:58:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 05:58:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 17 Jun 2020 05:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:245c4e26db07a2cb02b557ee0489110049d085365da3d831687f78dd82dd7a4b`  
		Last Modified: Wed, 17 Jun 2020 06:12:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08346bcdc43d5faa37eea1e6f047728863a5231825d5686a10a89beec62fbc75`  
		Last Modified: Wed, 17 Jun 2020 06:12:53 GMT  
		Size: 119.3 MB (119258493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f6075854d914bd6766e5f1908373638bc3fece230f0b7813270cad5bdd956`  
		Last Modified: Wed, 17 Jun 2020 06:12:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9923e5a7c484cdbbf5c431c2da18ad74641acbc32b9420d6d8a228f8fd31bad`  
		Last Modified: Wed, 17 Jun 2020 06:13:11 GMT  
		Size: 66.6 MB (66568404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f8ec5389a7d011ec55a2d0372adf259823854b4fce22cd5d48537828936f67`  
		Last Modified: Wed, 17 Jun 2020 06:12:59 GMT  
		Size: 180.2 KB (180189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bb11dec0824d907902ed501cbcbedc7196ccc74db319ec499e755c93382dc4`  
		Last Modified: Wed, 17 Jun 2020 06:12:58 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed85523e676152ce0947a2ba2d1a331966df822d7adb24efaf2e83428ffb63e8`  
		Last Modified: Wed, 17 Jun 2020 06:13:02 GMT  
		Size: 10.3 MB (10269425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6922e97d4707ead69720897d428b3d12d2dd0c3c0297e76612210525c46eb277
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207756090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e57654f926d8d72c65cc0ec5d1511c777820c38ebc25ca6d9ea0be2cb08779`
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
# Wed, 17 Jun 2020 04:25:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 04:25:44 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 04:25:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 04:25:49 GMT
ENV ROS_DISTRO=foxy
# Wed, 17 Jun 2020 04:27:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:28:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 04:28:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 04:28:03 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 04:28:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:29:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 04:29:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 17 Jun 2020 04:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:449fc159008401ac37e72ba47ebe0af89cd7453d6fba04661d8bd4f84e9e77d5`  
		Last Modified: Wed, 17 Jun 2020 04:48:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aae1e5bf9aaf21197fb06b568ef047dee2aaf77dd4439f22f6e1d62410354a2`  
		Last Modified: Wed, 17 Jun 2020 04:49:04 GMT  
		Size: 103.5 MB (103476015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cb414aaa1eccb6d043b3818b1b3401bf130d11b0acfd6a4c09d0054e056db9`  
		Last Modified: Wed, 17 Jun 2020 04:48:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360d431e7e8db907b4f2f43f0b7a8f6ecac91c09391f18a4091378ecc2ef3a07`  
		Last Modified: Wed, 17 Jun 2020 04:49:28 GMT  
		Size: 60.9 MB (60921173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9afec3ea5cb5cf7196137a69dee20480d64f4ca1f1785da80998b0af1e2f5`  
		Last Modified: Wed, 17 Jun 2020 04:49:11 GMT  
		Size: 180.3 KB (180253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf47ffa202ffa7c6889bbce778e8c350a4d077669f8d953200e672ae46ec4537`  
		Last Modified: Wed, 17 Jun 2020 04:49:11 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ab7b2070961e9d95c50e8ef958a51196d293a9b65691f7900b6a9bcfafcd5f`  
		Last Modified: Wed, 17 Jun 2020 04:49:15 GMT  
		Size: 9.3 MB (9289235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
