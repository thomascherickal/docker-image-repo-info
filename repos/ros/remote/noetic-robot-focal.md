## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:ea2f92288d891ba89b7b4842df8260c4b75867116791f41a4132d84371299733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:66bff5ec38f2ea099c660fc7564a827b3a4577c7a5dc6ea9e977ea18d1af4cb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.7 MB (350651474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee72109b0e9bae6e08c0c7a5fa837e7f9e8c53db9d5005b11e84f7e8a71bbc0`
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
# Thu, 26 Nov 2020 01:59:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 26 Nov 2020 01:59:26 GMT
ENV LANG=C.UTF-8
# Thu, 26 Nov 2020 01:59:26 GMT
ENV LC_ALL=C.UTF-8
# Thu, 26 Nov 2020 01:59:27 GMT
ENV ROS_DISTRO=noetic
# Thu, 26 Nov 2020 02:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:01:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 26 Nov 2020 02:01:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 26 Nov 2020 02:01:39 GMT
CMD ["bash"]
# Thu, 26 Nov 2020 02:02:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:02:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 26 Nov 2020 02:03:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:04:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:fe0e196c1a50c53d17a36354c41633bdd29372ea148fb375ca655cfb0a1b43e3`  
		Last Modified: Thu, 26 Nov 2020 02:31:31 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423eb030ae8ce9bdfafdc9d18416da92574292087407526dd3c13cdbbf03c502`  
		Last Modified: Thu, 26 Nov 2020 02:32:15 GMT  
		Size: 173.2 MB (173245254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ee818e2e9a82cf7ce17415df0fa12eb754edae6c57ebcd5dab1749cf1ebf51`  
		Last Modified: Thu, 26 Nov 2020 02:31:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f041c4166db495e54124411c6fe377cf6946475d17bec14bed4628142df575`  
		Last Modified: Thu, 26 Nov 2020 02:32:30 GMT  
		Size: 46.4 MB (46381868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f3f32b66d84b272423a7f83aebb999decd4753f615856092b6204c3efdab1e`  
		Last Modified: Thu, 26 Nov 2020 02:32:20 GMT  
		Size: 252.1 KB (252121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9483a9a8e4926648acf928efba53f2886ab578def0d49d478d382ff50c5bdfd`  
		Last Modified: Thu, 26 Nov 2020 02:32:37 GMT  
		Size: 79.6 MB (79590716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51a8a177696d6ebe90bd1c91fd72228fd346f643e5fc983830e8b056918d0b3`  
		Last Modified: Thu, 26 Nov 2020 02:32:47 GMT  
		Size: 15.9 MB (15889593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:124c8158ebbb779f0edb69a5ec5e95f6d5a7f96b9d18241741f192320816408a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297749131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d20f0e62a06ae59d65f8434731c3660f2122b449b46463c57e53a83510f9b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:15:51 GMT
ADD file:874b5c952a766aaeff6c0d01f72a2644501ac0c8ab3ea3eef70339f045f09897 in / 
# Thu, 21 Jan 2021 03:15:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:15:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:15:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:15:59 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:41:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:42:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 04:42:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 21 Jan 2021 04:42:22 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 04:42:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 21 Jan 2021 04:42:27 GMT
ENV ROS_DISTRO=noetic
# Thu, 21 Jan 2021 04:44:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:44:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 21 Jan 2021 04:44:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 21 Jan 2021 04:45:00 GMT
CMD ["bash"]
# Thu, 21 Jan 2021 04:45:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:45:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 21 Jan 2021 04:46:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:47:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5b689817f397e49f6802d29f6e262a92b16ef6fd29e0dbe7c957ecf60421c1f`  
		Last Modified: Thu, 21 Jan 2021 03:18:26 GMT  
		Size: 24.0 MB (24043427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b105a146cef196c701ff39cc8b99248972b0b02b544bb5fc1346bf37b870383`  
		Last Modified: Thu, 21 Jan 2021 03:18:19 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22943c6e232d1034beb778a2094ae7d8bb94122e5e562c65769abc93a3ab1731`  
		Last Modified: Thu, 21 Jan 2021 03:18:19 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da94c2e1ffe7a207cb16387dad3b7bdb14e1ae74ff5ebabe6670f20a2590bbd3`  
		Last Modified: Thu, 21 Jan 2021 05:16:04 GMT  
		Size: 1.2 MB (1183165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc0bd3c7c8507acfba5a1709d766b0fb7073f21a2abdc0fb08dc3513be90682`  
		Last Modified: Thu, 21 Jan 2021 05:16:03 GMT  
		Size: 4.7 MB (4676841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b65d68849907d97ed8c56594ed5c564b5b697d5c30b1d279fa96d856d8caaa`  
		Last Modified: Thu, 21 Jan 2021 05:16:00 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a72237a1f08d55965016589ac175e3d7390c84c942f8c1c65f1dafb899370c`  
		Last Modified: Thu, 21 Jan 2021 05:16:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec039649d5d1f6a5f97883f049f2cc038bebe026fbc0b5f5af534d4287d69eef`  
		Last Modified: Thu, 21 Jan 2021 05:16:59 GMT  
		Size: 157.2 MB (157173558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424cf09681c7cbde74a8bf71b7b5a7d6e0ed90babb5c8d1fb3637e66f75c4b97`  
		Last Modified: Thu, 21 Jan 2021 05:16:00 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62603737697bee97d0138f5851506613d2bb349f41f56cbc6ec5e4ebf9c6c56d`  
		Last Modified: Thu, 21 Jan 2021 05:17:23 GMT  
		Size: 35.8 MB (35830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9faeee5bc3b322e38e5f85b82d6b523988bdcf94354f52cdaa8b3df211b939`  
		Last Modified: Thu, 21 Jan 2021 05:17:13 GMT  
		Size: 269.1 KB (269099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15990ce210679aeb22235099a668c7637cf0f92012187ad39e9ab509724c140`  
		Last Modified: Thu, 21 Jan 2021 05:17:36 GMT  
		Size: 60.5 MB (60482276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4df1fb4fb79b025ec1afc934bf3db0407330905ebd93b0cd355ccc66f4f57d3`  
		Last Modified: Thu, 21 Jan 2021 05:17:55 GMT  
		Size: 14.1 MB (14087207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3f413e3209e7a30ce3685901051bca99b34ef3577d9bc83787c7b33d685e4ba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329943092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09b2dac37afae23df8edaec74722705c0ea29ff53582ad64dabfe302051334c`
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
# Thu, 26 Nov 2020 00:09:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 26 Nov 2020 00:09:53 GMT
ENV LANG=C.UTF-8
# Thu, 26 Nov 2020 00:09:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 26 Nov 2020 00:09:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 26 Nov 2020 00:12:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:12:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 26 Nov 2020 00:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 26 Nov 2020 00:12:09 GMT
CMD ["bash"]
# Thu, 26 Nov 2020 00:12:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:12:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 26 Nov 2020 00:13:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:9820d378995c3063b66eb48a344c33a2c1f32ff689424487c298fa1c10349f05`  
		Last Modified: Thu, 26 Nov 2020 01:10:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e677b6e8561be320411a4a62b55c88a3d8f63fc5c9998db3801c3b0a88756`  
		Last Modified: Thu, 26 Nov 2020 01:11:19 GMT  
		Size: 167.7 MB (167722399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0378bdc1c8f187821a9b08d288a24f45bdfb119f26f77b0f3cf9adfdb553773e`  
		Last Modified: Thu, 26 Nov 2020 01:10:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79529ea52f10728327e4c62428a86ee3c615c90189bb63801fb8b7dd4378119b`  
		Last Modified: Thu, 26 Nov 2020 01:11:38 GMT  
		Size: 40.7 MB (40651718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bccdb4db1b06460c6a872413d9d91ae66093a6b7d6414af901d256ad257944`  
		Last Modified: Thu, 26 Nov 2020 01:11:28 GMT  
		Size: 252.2 KB (252184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6113a9e8958c4cf6594645de3e6725b3079ca344d6e148a0b31a6e60c5aeaf38`  
		Last Modified: Thu, 26 Nov 2020 01:11:47 GMT  
		Size: 72.0 MB (71974190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6bb32b1ea0bbb28ff91e2982600935ab01476f90fbf2b36b4f1221ce580fa4`  
		Last Modified: Thu, 26 Nov 2020 01:12:01 GMT  
		Size: 15.5 MB (15478321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
