## `ros:foxy`

```console
$ docker pull ros@sha256:f80630ff210d0f7abc95e2b58c00cd2394c521a67bb7a43961fbd73bb38fe306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:49cc70271b0b2d5638e9dd6a1f2803a367c7e653bd5024628c7c69d5b06e3782
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231712484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8957756f529fc629a7e5e520853c4b704bed6f7ad2eedc660ab6b07d7a04d05c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:37:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:34:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:34:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 01:55:03 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 17 Sep 2020 01:55:03 GMT
ENV LANG=C.UTF-8
# Thu, 17 Sep 2020 01:55:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Sep 2020 01:55:03 GMT
ENV ROS_DISTRO=foxy
# Thu, 17 Sep 2020 01:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:56:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 17 Sep 2020 01:56:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 01:56:36 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 01:57:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:57:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 01:57:28 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 17 Sep 2020 01:57:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd43f844b454143fefb276b0d47a08c31858e330ffeceef21130f4f907c2691e`  
		Last Modified: Thu, 17 Sep 2020 00:52:12 GMT  
		Size: 1.2 MB (1176444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25929632fd5b65202802f96157aaae95b55bcb587a77c708a4d63e5d2100db09`  
		Last Modified: Thu, 17 Sep 2020 02:08:15 GMT  
		Size: 5.5 MB (5547001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa5e6421658a99911cb295c7f31b4f12e6a3f61860c7814b87cddc1a985e215`  
		Last Modified: Thu, 17 Sep 2020 02:08:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b62c6d955edf0b3d12ec0e851b2c8e6901c44cc4798da5c77c35bef01209da`  
		Last Modified: Thu, 17 Sep 2020 02:14:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2b66304789e3439a1a20d7b92034ea5374768eaf73ae3e04753c003723f421`  
		Last Modified: Thu, 17 Sep 2020 02:15:26 GMT  
		Size: 119.4 MB (119372008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8699c1a075cf2f62a951eeceb18b4ce20fda71db84ea44010eb43b048e05395`  
		Last Modified: Thu, 17 Sep 2020 02:14:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be667231523248f5b6ee4b7ba9186c2b0a222fabc356c2db494f0d49f20a2a10`  
		Last Modified: Thu, 17 Sep 2020 02:15:44 GMT  
		Size: 66.6 MB (66579269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788b1cb1fa2e61d94fe656ba09e23d528fb6f5a71e06779d9830eb37568fbee2`  
		Last Modified: Thu, 17 Sep 2020 02:15:30 GMT  
		Size: 193.9 KB (193940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847c23480de1510c22a46ffd4eced3735b12b38ace5c71f5129ab5060cfffd03`  
		Last Modified: Thu, 17 Sep 2020 02:15:30 GMT  
		Size: 2.0 KB (2007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1090a7388af6170aa8569474e1ac5ab7f89c27eca15f4b287fa33bba6df5b285`  
		Last Modified: Thu, 17 Sep 2020 02:15:34 GMT  
		Size: 10.3 MB (10281806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ffba52a87a0047904b6f4258503b53f17dab997ce29dfb78f3fb1ab02e4d80b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.9 MB (207856810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e21c746ddd5cf8dc3984bcfcbf28fbad28633e9645567370976390b3c610ec9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:30:23 GMT
ADD file:a332d170aaa2d4c28c85289b62d33de68027ce4d6b0616292ee2252dfdf2628b in / 
# Wed, 19 Aug 2020 21:30:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:30:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:30:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:30:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:24:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:25:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:25:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:47:03 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 19 Aug 2020 23:47:04 GMT
ENV LANG=C.UTF-8
# Wed, 19 Aug 2020 23:47:05 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 Aug 2020 23:47:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 19 Aug 2020 23:49:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:49:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 19 Aug 2020 23:49:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 23:49:19 GMT
CMD ["bash"]
# Wed, 19 Aug 2020 23:50:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:50:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 19 Aug 2020 23:51:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 19 Aug 2020 23:51:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61ca5746b6ffb91caaaa0eb4b9678ae147ad24bd40ac203758a90af376976f98`  
		Last Modified: Wed, 29 Jul 2020 08:25:33 GMT  
		Size: 27.2 MB (27162745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d07cd4558d7ea5ba152468ba362cbf62a56cfab14976467187d3943013a932`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 32.3 KB (32335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ef536d7ca531a0dce4a70ac7ad7d9b7ed27c56c7f0953bbec370e4299b951`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d5c7c4a6e93095601576a7663dde336974f6a96329ae2a613511662ed8744`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4083e46f11503c80095b52102ecdb34f1f88359ab6776daee0f399dd71c60372`  
		Last Modified: Thu, 20 Aug 2020 00:11:52 GMT  
		Size: 1.2 MB (1176161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7764603dd05c49038a524211ad7ceb67d2670cab2505beea1af401cca1e779`  
		Last Modified: Thu, 20 Aug 2020 00:11:48 GMT  
		Size: 5.5 MB (5511900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036f7ca74d2d186cd0993ac4fc4b9cef66c4777f93b40d28474a8e487429514f`  
		Last Modified: Thu, 20 Aug 2020 00:11:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570794c6903fc984991682fb63b7f759d52aa83c56c5a79a9d052dc142414524`  
		Last Modified: Thu, 20 Aug 2020 00:20:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfe2c97a91ece4c8c65879e94f05bb84074d61dc62373e8b0d236186be5ff4e`  
		Last Modified: Thu, 20 Aug 2020 00:20:35 GMT  
		Size: 103.5 MB (103548323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b4d5cd498be33da61888884aea8cc59b55d642839c5eba1747d3a8c6786f8`  
		Last Modified: Thu, 20 Aug 2020 00:20:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4c3d8d25318eb83758d2d30ed2f1d9fd5e6b1f3dfccdeccfdf454a0143d1bd`  
		Last Modified: Thu, 20 Aug 2020 00:21:20 GMT  
		Size: 60.9 MB (60932505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2965af5207117f40fe6f9d41af3649d263a565580ad7e4907a045951a9170d7`  
		Last Modified: Thu, 20 Aug 2020 00:20:45 GMT  
		Size: 191.2 KB (191246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8013e5d039e1fc0dc8abedd1d18ff0699a56be442911b93da40c9ad8c498cf06`  
		Last Modified: Thu, 20 Aug 2020 00:20:45 GMT  
		Size: 2.1 KB (2071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50e78bc3e96c1568399cf4ef0d0715cbb0e1eb5c810899b33aa7500a7b960b`  
		Last Modified: Thu, 20 Aug 2020 00:20:49 GMT  
		Size: 9.3 MB (9296651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
