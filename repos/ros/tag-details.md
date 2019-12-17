<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:crystal`](#roscrystal)
-	[`ros:crystal-ros-base`](#roscrystal-ros-base)
-	[`ros:crystal-ros-base-bionic`](#roscrystal-ros-base-bionic)
-	[`ros:crystal-ros-core`](#roscrystal-ros-core)
-	[`ros:crystal-ros-core-bionic`](#roscrystal-ros-core-bionic)
-	[`ros:dashing`](#rosdashing)
-	[`ros:dashing-ros-base`](#rosdashing-ros-base)
-	[`ros:dashing-ros-base-bionic`](#rosdashing-ros-base-bionic)
-	[`ros:dashing-ros-core`](#rosdashing-ros-core)
-	[`ros:dashing-ros-core-bionic`](#rosdashing-ros-core-bionic)
-	[`ros:eloquent`](#roseloquent)
-	[`ros:eloquent-ros-base`](#roseloquent-ros-base)
-	[`ros:eloquent-ros-base-bionic`](#roseloquent-ros-base-bionic)
-	[`ros:eloquent-ros-core`](#roseloquent-ros-core)
-	[`ros:eloquent-ros-core-bionic`](#roseloquent-ros-core-bionic)
-	[`ros:kinetic`](#roskinetic)
-	[`ros:kinetic-perception`](#roskinetic-perception)
-	[`ros:kinetic-perception-xenial`](#roskinetic-perception-xenial)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-robot-xenial`](#roskinetic-robot-xenial)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic-ros-base-xenial`](#roskinetic-ros-base-xenial)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-core-xenial`](#roskinetic-ros-core-xenial)
-	[`ros:latest`](#roslatest)
-	[`ros:melodic`](#rosmelodic)
-	[`ros:melodic-perception`](#rosmelodic-perception)
-	[`ros:melodic-perception-bionic`](#rosmelodic-perception-bionic)
-	[`ros:melodic-perception-stretch`](#rosmelodic-perception-stretch)
-	[`ros:melodic-robot`](#rosmelodic-robot)
-	[`ros:melodic-robot-bionic`](#rosmelodic-robot-bionic)
-	[`ros:melodic-robot-stretch`](#rosmelodic-robot-stretch)
-	[`ros:melodic-ros-base`](#rosmelodic-ros-base)
-	[`ros:melodic-ros-base-bionic`](#rosmelodic-ros-base-bionic)
-	[`ros:melodic-ros-base-stretch`](#rosmelodic-ros-base-stretch)
-	[`ros:melodic-ros-core`](#rosmelodic-ros-core)
-	[`ros:melodic-ros-core-bionic`](#rosmelodic-ros-core-bionic)
-	[`ros:melodic-ros-core-stretch`](#rosmelodic-ros-core-stretch)

## `ros:crystal`

```console
$ docker pull ros@sha256:91afaa71b60e6f9f21681d9f5d9eff9463bb1f933f6d7b5908847f9abf203b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal` - linux; amd64

```console
$ docker pull ros@sha256:fce2c16c74fbeecfb17eba5379433d8dbe2e3b7a5dc1d53534f4a5caeb85cf6f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.8 MB (264762066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fbab0b60b9298baae4db2cc8d4a082f016d05b79bc8cb4ee1036235c181a9ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:23:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 16 Dec 2019 23:23:54 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Mon, 16 Dec 2019 23:24:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LANG=C.UTF-8
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LC_ALL=C.UTF-8
# Mon, 16 Dec 2019 23:24:48 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Mon, 16 Dec 2019 23:24:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 16 Dec 2019 23:24:54 GMT
RUN pip3 install -U     argcomplete
# Mon, 16 Dec 2019 23:24:54 GMT
ENV ROS_DISTRO=crystal
# Mon, 16 Dec 2019 23:26:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:26:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:26:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:26:27 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:26:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0f83d600db071c4afd65ed928e934bd7a7ccd1527a57abb5df75a77b7340f`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 2.8 KB (2817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee015464f229a4e4886fc8d04792ab2c361b89518269391b251584442fea487d`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8d6e44ec40df9780cb302eb69816b45063f54a67bef09a8e1afbb22a509eb`  
		Last Modified: Mon, 16 Dec 2019 23:29:11 GMT  
		Size: 28.4 MB (28395376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bbb5a72deabcc91fa0d2a77e71a5fbdfdbf181870a067f1400b2b8fcf89166`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1000.0 KB (1000024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7d5cbfef7d0510db866bb8e7a2322b3dbfa3e7df69881540f2580eaefd19e1`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08cddc77954ad873b25d252f1e59a6cceb39b0ab0b05c3607e5267b62b023e6`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 105.6 KB (105622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536966aacbe67979488cd6b0ed07da0f52d216fe1c529808ea320092e801c1e`  
		Last Modified: Mon, 16 Dec 2019 23:29:16 GMT  
		Size: 52.5 MB (52508107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a47251011b2d1d15ef49dba61ef4051343dc3509edfc9627234857e05fea242`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3f4959e124ea4b6333f538ac861d6ceaa2bd75073019394f8b1a21e5aac10a`  
		Last Modified: Mon, 16 Dec 2019 23:29:40 GMT  
		Size: 3.2 MB (3179988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7370dda5a22d49879ea9438b3cd411ac6d02b5fe769ea76180fa8860d05cea3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194795431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccebe0512ebe874f57bba35dfe034aac2c96c4d357a530c8b25777f161954dda`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:04:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 17 Dec 2019 00:04:44 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 17 Dec 2019 00:06:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:06:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Dec 2019 00:06:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Dec 2019 00:07:17 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Tue, 17 Dec 2019 00:07:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 17 Dec 2019 00:07:33 GMT
RUN pip3 install -U     argcomplete
# Tue, 17 Dec 2019 00:07:34 GMT
ENV ROS_DISTRO=crystal
# Tue, 17 Dec 2019 00:09:12 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:09:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:09:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:09:16 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:09:46 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3425f37b9d1cbef29d81dd9cdc45f35a5408b141264eb244f40cf5e624e9ad5`  
		Last Modified: Tue, 17 Dec 2019 00:16:36 GMT  
		Size: 2.8 KB (2816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae32a479784fb212a29e3f02a85d6e1d3916f1779761941d9c4b1fd47674d44`  
		Last Modified: Tue, 17 Dec 2019 00:16:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66968e02d984d1d72504b5dfd3f781ed4556c844d615dc328121488a8895e95f`  
		Last Modified: Tue, 17 Dec 2019 00:16:43 GMT  
		Size: 27.1 MB (27082001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493123ae69dfec6357246a291368fb34fe571b91a3af404e02a7f6274f42f11`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1000.1 KB (1000087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554f73c496fd62def781836effa8818f3bc62a01427e55209d530c31f41832e`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0fbc1e5bf1cbaceb2e30cf39bd5664c96b2bf0e4f64cfd6a4e0d0ab8a4ea90`  
		Last Modified: Tue, 17 Dec 2019 00:16:34 GMT  
		Size: 105.8 KB (105750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9bd960b18352a35d0e3621b0b93bf30fe6a4af0e6f3b3ee320a0066ab1fd6e`  
		Last Modified: Tue, 17 Dec 2019 00:16:49 GMT  
		Size: 41.7 MB (41714866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346fcafff6d4d08692fb7d8093db676fa14fe6580b7dc9f988f88d1fac9a55c3`  
		Last Modified: Tue, 17 Dec 2019 00:16:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0397039aa9721b6085c228bd7a244b82d8d7af697517cc5531dce03b6905d1`  
		Last Modified: Tue, 17 Dec 2019 00:17:00 GMT  
		Size: 2.9 MB (2942755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-base`

```console
$ docker pull ros@sha256:91afaa71b60e6f9f21681d9f5d9eff9463bb1f933f6d7b5908847f9abf203b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:fce2c16c74fbeecfb17eba5379433d8dbe2e3b7a5dc1d53534f4a5caeb85cf6f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.8 MB (264762066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fbab0b60b9298baae4db2cc8d4a082f016d05b79bc8cb4ee1036235c181a9ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:23:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 16 Dec 2019 23:23:54 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Mon, 16 Dec 2019 23:24:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LANG=C.UTF-8
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LC_ALL=C.UTF-8
# Mon, 16 Dec 2019 23:24:48 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Mon, 16 Dec 2019 23:24:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 16 Dec 2019 23:24:54 GMT
RUN pip3 install -U     argcomplete
# Mon, 16 Dec 2019 23:24:54 GMT
ENV ROS_DISTRO=crystal
# Mon, 16 Dec 2019 23:26:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:26:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:26:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:26:27 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:26:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0f83d600db071c4afd65ed928e934bd7a7ccd1527a57abb5df75a77b7340f`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 2.8 KB (2817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee015464f229a4e4886fc8d04792ab2c361b89518269391b251584442fea487d`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8d6e44ec40df9780cb302eb69816b45063f54a67bef09a8e1afbb22a509eb`  
		Last Modified: Mon, 16 Dec 2019 23:29:11 GMT  
		Size: 28.4 MB (28395376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bbb5a72deabcc91fa0d2a77e71a5fbdfdbf181870a067f1400b2b8fcf89166`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1000.0 KB (1000024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7d5cbfef7d0510db866bb8e7a2322b3dbfa3e7df69881540f2580eaefd19e1`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08cddc77954ad873b25d252f1e59a6cceb39b0ab0b05c3607e5267b62b023e6`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 105.6 KB (105622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536966aacbe67979488cd6b0ed07da0f52d216fe1c529808ea320092e801c1e`  
		Last Modified: Mon, 16 Dec 2019 23:29:16 GMT  
		Size: 52.5 MB (52508107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a47251011b2d1d15ef49dba61ef4051343dc3509edfc9627234857e05fea242`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3f4959e124ea4b6333f538ac861d6ceaa2bd75073019394f8b1a21e5aac10a`  
		Last Modified: Mon, 16 Dec 2019 23:29:40 GMT  
		Size: 3.2 MB (3179988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7370dda5a22d49879ea9438b3cd411ac6d02b5fe769ea76180fa8860d05cea3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194795431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccebe0512ebe874f57bba35dfe034aac2c96c4d357a530c8b25777f161954dda`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:04:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 17 Dec 2019 00:04:44 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 17 Dec 2019 00:06:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:06:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Dec 2019 00:06:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Dec 2019 00:07:17 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Tue, 17 Dec 2019 00:07:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 17 Dec 2019 00:07:33 GMT
RUN pip3 install -U     argcomplete
# Tue, 17 Dec 2019 00:07:34 GMT
ENV ROS_DISTRO=crystal
# Tue, 17 Dec 2019 00:09:12 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:09:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:09:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:09:16 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:09:46 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3425f37b9d1cbef29d81dd9cdc45f35a5408b141264eb244f40cf5e624e9ad5`  
		Last Modified: Tue, 17 Dec 2019 00:16:36 GMT  
		Size: 2.8 KB (2816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae32a479784fb212a29e3f02a85d6e1d3916f1779761941d9c4b1fd47674d44`  
		Last Modified: Tue, 17 Dec 2019 00:16:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66968e02d984d1d72504b5dfd3f781ed4556c844d615dc328121488a8895e95f`  
		Last Modified: Tue, 17 Dec 2019 00:16:43 GMT  
		Size: 27.1 MB (27082001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493123ae69dfec6357246a291368fb34fe571b91a3af404e02a7f6274f42f11`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1000.1 KB (1000087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554f73c496fd62def781836effa8818f3bc62a01427e55209d530c31f41832e`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0fbc1e5bf1cbaceb2e30cf39bd5664c96b2bf0e4f64cfd6a4e0d0ab8a4ea90`  
		Last Modified: Tue, 17 Dec 2019 00:16:34 GMT  
		Size: 105.8 KB (105750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9bd960b18352a35d0e3621b0b93bf30fe6a4af0e6f3b3ee320a0066ab1fd6e`  
		Last Modified: Tue, 17 Dec 2019 00:16:49 GMT  
		Size: 41.7 MB (41714866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346fcafff6d4d08692fb7d8093db676fa14fe6580b7dc9f988f88d1fac9a55c3`  
		Last Modified: Tue, 17 Dec 2019 00:16:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0397039aa9721b6085c228bd7a244b82d8d7af697517cc5531dce03b6905d1`  
		Last Modified: Tue, 17 Dec 2019 00:17:00 GMT  
		Size: 2.9 MB (2942755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-base-bionic`

```console
$ docker pull ros@sha256:91afaa71b60e6f9f21681d9f5d9eff9463bb1f933f6d7b5908847f9abf203b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:fce2c16c74fbeecfb17eba5379433d8dbe2e3b7a5dc1d53534f4a5caeb85cf6f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.8 MB (264762066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fbab0b60b9298baae4db2cc8d4a082f016d05b79bc8cb4ee1036235c181a9ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:23:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 16 Dec 2019 23:23:54 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Mon, 16 Dec 2019 23:24:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LANG=C.UTF-8
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LC_ALL=C.UTF-8
# Mon, 16 Dec 2019 23:24:48 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Mon, 16 Dec 2019 23:24:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 16 Dec 2019 23:24:54 GMT
RUN pip3 install -U     argcomplete
# Mon, 16 Dec 2019 23:24:54 GMT
ENV ROS_DISTRO=crystal
# Mon, 16 Dec 2019 23:26:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:26:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:26:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:26:27 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:26:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0f83d600db071c4afd65ed928e934bd7a7ccd1527a57abb5df75a77b7340f`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 2.8 KB (2817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee015464f229a4e4886fc8d04792ab2c361b89518269391b251584442fea487d`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8d6e44ec40df9780cb302eb69816b45063f54a67bef09a8e1afbb22a509eb`  
		Last Modified: Mon, 16 Dec 2019 23:29:11 GMT  
		Size: 28.4 MB (28395376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bbb5a72deabcc91fa0d2a77e71a5fbdfdbf181870a067f1400b2b8fcf89166`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1000.0 KB (1000024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7d5cbfef7d0510db866bb8e7a2322b3dbfa3e7df69881540f2580eaefd19e1`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08cddc77954ad873b25d252f1e59a6cceb39b0ab0b05c3607e5267b62b023e6`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 105.6 KB (105622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536966aacbe67979488cd6b0ed07da0f52d216fe1c529808ea320092e801c1e`  
		Last Modified: Mon, 16 Dec 2019 23:29:16 GMT  
		Size: 52.5 MB (52508107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a47251011b2d1d15ef49dba61ef4051343dc3509edfc9627234857e05fea242`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3f4959e124ea4b6333f538ac861d6ceaa2bd75073019394f8b1a21e5aac10a`  
		Last Modified: Mon, 16 Dec 2019 23:29:40 GMT  
		Size: 3.2 MB (3179988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b7370dda5a22d49879ea9438b3cd411ac6d02b5fe769ea76180fa8860d05cea3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194795431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccebe0512ebe874f57bba35dfe034aac2c96c4d357a530c8b25777f161954dda`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:04:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 17 Dec 2019 00:04:44 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 17 Dec 2019 00:06:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:06:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Dec 2019 00:06:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Dec 2019 00:07:17 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Tue, 17 Dec 2019 00:07:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 17 Dec 2019 00:07:33 GMT
RUN pip3 install -U     argcomplete
# Tue, 17 Dec 2019 00:07:34 GMT
ENV ROS_DISTRO=crystal
# Tue, 17 Dec 2019 00:09:12 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:09:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:09:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:09:16 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:09:46 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3425f37b9d1cbef29d81dd9cdc45f35a5408b141264eb244f40cf5e624e9ad5`  
		Last Modified: Tue, 17 Dec 2019 00:16:36 GMT  
		Size: 2.8 KB (2816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae32a479784fb212a29e3f02a85d6e1d3916f1779761941d9c4b1fd47674d44`  
		Last Modified: Tue, 17 Dec 2019 00:16:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66968e02d984d1d72504b5dfd3f781ed4556c844d615dc328121488a8895e95f`  
		Last Modified: Tue, 17 Dec 2019 00:16:43 GMT  
		Size: 27.1 MB (27082001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493123ae69dfec6357246a291368fb34fe571b91a3af404e02a7f6274f42f11`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1000.1 KB (1000087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554f73c496fd62def781836effa8818f3bc62a01427e55209d530c31f41832e`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0fbc1e5bf1cbaceb2e30cf39bd5664c96b2bf0e4f64cfd6a4e0d0ab8a4ea90`  
		Last Modified: Tue, 17 Dec 2019 00:16:34 GMT  
		Size: 105.8 KB (105750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9bd960b18352a35d0e3621b0b93bf30fe6a4af0e6f3b3ee320a0066ab1fd6e`  
		Last Modified: Tue, 17 Dec 2019 00:16:49 GMT  
		Size: 41.7 MB (41714866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346fcafff6d4d08692fb7d8093db676fa14fe6580b7dc9f988f88d1fac9a55c3`  
		Last Modified: Tue, 17 Dec 2019 00:16:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0397039aa9721b6085c228bd7a244b82d8d7af697517cc5531dce03b6905d1`  
		Last Modified: Tue, 17 Dec 2019 00:17:00 GMT  
		Size: 2.9 MB (2942755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-core`

```console
$ docker pull ros@sha256:41e82e1e33f7a74d41ad9daad9eb1016c8a46ed042a50bbcfc97dbb4226bf248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:42c56790a74fb68e2ebf0c6bdec1389a1ae875edb4ab237653da561ee668973c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261582078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d302c2b678e00cbdbbf490f34c6da26f1910bdebbfd26bd04f17b0b6bb4c57b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:23:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 16 Dec 2019 23:23:54 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Mon, 16 Dec 2019 23:24:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LANG=C.UTF-8
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LC_ALL=C.UTF-8
# Mon, 16 Dec 2019 23:24:48 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Mon, 16 Dec 2019 23:24:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 16 Dec 2019 23:24:54 GMT
RUN pip3 install -U     argcomplete
# Mon, 16 Dec 2019 23:24:54 GMT
ENV ROS_DISTRO=crystal
# Mon, 16 Dec 2019 23:26:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:26:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:26:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:26:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0f83d600db071c4afd65ed928e934bd7a7ccd1527a57abb5df75a77b7340f`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 2.8 KB (2817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee015464f229a4e4886fc8d04792ab2c361b89518269391b251584442fea487d`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8d6e44ec40df9780cb302eb69816b45063f54a67bef09a8e1afbb22a509eb`  
		Last Modified: Mon, 16 Dec 2019 23:29:11 GMT  
		Size: 28.4 MB (28395376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bbb5a72deabcc91fa0d2a77e71a5fbdfdbf181870a067f1400b2b8fcf89166`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1000.0 KB (1000024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7d5cbfef7d0510db866bb8e7a2322b3dbfa3e7df69881540f2580eaefd19e1`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08cddc77954ad873b25d252f1e59a6cceb39b0ab0b05c3607e5267b62b023e6`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 105.6 KB (105622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536966aacbe67979488cd6b0ed07da0f52d216fe1c529808ea320092e801c1e`  
		Last Modified: Mon, 16 Dec 2019 23:29:16 GMT  
		Size: 52.5 MB (52508107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a47251011b2d1d15ef49dba61ef4051343dc3509edfc9627234857e05fea242`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:54090cb853c63d927c678f1addf1a8761ec1289392d416eb9253d85413941487
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191852676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208c3376b57b404ec4a9fc63bd4b1077f43806962edceddfe500c5009bdc75c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:04:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 17 Dec 2019 00:04:44 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 17 Dec 2019 00:06:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:06:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Dec 2019 00:06:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Dec 2019 00:07:17 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Tue, 17 Dec 2019 00:07:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 17 Dec 2019 00:07:33 GMT
RUN pip3 install -U     argcomplete
# Tue, 17 Dec 2019 00:07:34 GMT
ENV ROS_DISTRO=crystal
# Tue, 17 Dec 2019 00:09:12 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:09:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:09:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:09:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3425f37b9d1cbef29d81dd9cdc45f35a5408b141264eb244f40cf5e624e9ad5`  
		Last Modified: Tue, 17 Dec 2019 00:16:36 GMT  
		Size: 2.8 KB (2816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae32a479784fb212a29e3f02a85d6e1d3916f1779761941d9c4b1fd47674d44`  
		Last Modified: Tue, 17 Dec 2019 00:16:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66968e02d984d1d72504b5dfd3f781ed4556c844d615dc328121488a8895e95f`  
		Last Modified: Tue, 17 Dec 2019 00:16:43 GMT  
		Size: 27.1 MB (27082001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493123ae69dfec6357246a291368fb34fe571b91a3af404e02a7f6274f42f11`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1000.1 KB (1000087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554f73c496fd62def781836effa8818f3bc62a01427e55209d530c31f41832e`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0fbc1e5bf1cbaceb2e30cf39bd5664c96b2bf0e4f64cfd6a4e0d0ab8a4ea90`  
		Last Modified: Tue, 17 Dec 2019 00:16:34 GMT  
		Size: 105.8 KB (105750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9bd960b18352a35d0e3621b0b93bf30fe6a4af0e6f3b3ee320a0066ab1fd6e`  
		Last Modified: Tue, 17 Dec 2019 00:16:49 GMT  
		Size: 41.7 MB (41714866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346fcafff6d4d08692fb7d8093db676fa14fe6580b7dc9f988f88d1fac9a55c3`  
		Last Modified: Tue, 17 Dec 2019 00:16:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-core-bionic`

```console
$ docker pull ros@sha256:41e82e1e33f7a74d41ad9daad9eb1016c8a46ed042a50bbcfc97dbb4226bf248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:42c56790a74fb68e2ebf0c6bdec1389a1ae875edb4ab237653da561ee668973c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261582078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d302c2b678e00cbdbbf490f34c6da26f1910bdebbfd26bd04f17b0b6bb4c57b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:23:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 16 Dec 2019 23:23:54 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Mon, 16 Dec 2019 23:24:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LANG=C.UTF-8
# Mon, 16 Dec 2019 23:24:33 GMT
ENV LC_ALL=C.UTF-8
# Mon, 16 Dec 2019 23:24:48 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Mon, 16 Dec 2019 23:24:52 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 16 Dec 2019 23:24:54 GMT
RUN pip3 install -U     argcomplete
# Mon, 16 Dec 2019 23:24:54 GMT
ENV ROS_DISTRO=crystal
# Mon, 16 Dec 2019 23:26:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:26:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:26:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:26:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0f83d600db071c4afd65ed928e934bd7a7ccd1527a57abb5df75a77b7340f`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 2.8 KB (2817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee015464f229a4e4886fc8d04792ab2c361b89518269391b251584442fea487d`  
		Last Modified: Mon, 16 Dec 2019 23:29:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8d6e44ec40df9780cb302eb69816b45063f54a67bef09a8e1afbb22a509eb`  
		Last Modified: Mon, 16 Dec 2019 23:29:11 GMT  
		Size: 28.4 MB (28395376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bbb5a72deabcc91fa0d2a77e71a5fbdfdbf181870a067f1400b2b8fcf89166`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1000.0 KB (1000024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7d5cbfef7d0510db866bb8e7a2322b3dbfa3e7df69881540f2580eaefd19e1`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08cddc77954ad873b25d252f1e59a6cceb39b0ab0b05c3607e5267b62b023e6`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 105.6 KB (105622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536966aacbe67979488cd6b0ed07da0f52d216fe1c529808ea320092e801c1e`  
		Last Modified: Mon, 16 Dec 2019 23:29:16 GMT  
		Size: 52.5 MB (52508107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a47251011b2d1d15ef49dba61ef4051343dc3509edfc9627234857e05fea242`  
		Last Modified: Mon, 16 Dec 2019 23:29:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:54090cb853c63d927c678f1addf1a8761ec1289392d416eb9253d85413941487
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191852676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208c3376b57b404ec4a9fc63bd4b1077f43806962edceddfe500c5009bdc75c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:04:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 17 Dec 2019 00:04:44 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Tue, 17 Dec 2019 00:06:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:06:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Dec 2019 00:06:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Dec 2019 00:07:17 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Tue, 17 Dec 2019 00:07:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 17 Dec 2019 00:07:33 GMT
RUN pip3 install -U     argcomplete
# Tue, 17 Dec 2019 00:07:34 GMT
ENV ROS_DISTRO=crystal
# Tue, 17 Dec 2019 00:09:12 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:09:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:09:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:09:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3425f37b9d1cbef29d81dd9cdc45f35a5408b141264eb244f40cf5e624e9ad5`  
		Last Modified: Tue, 17 Dec 2019 00:16:36 GMT  
		Size: 2.8 KB (2816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae32a479784fb212a29e3f02a85d6e1d3916f1779761941d9c4b1fd47674d44`  
		Last Modified: Tue, 17 Dec 2019 00:16:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66968e02d984d1d72504b5dfd3f781ed4556c844d615dc328121488a8895e95f`  
		Last Modified: Tue, 17 Dec 2019 00:16:43 GMT  
		Size: 27.1 MB (27082001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493123ae69dfec6357246a291368fb34fe571b91a3af404e02a7f6274f42f11`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1000.1 KB (1000087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554f73c496fd62def781836effa8818f3bc62a01427e55209d530c31f41832e`  
		Last Modified: Tue, 17 Dec 2019 00:16:33 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0fbc1e5bf1cbaceb2e30cf39bd5664c96b2bf0e4f64cfd6a4e0d0ab8a4ea90`  
		Last Modified: Tue, 17 Dec 2019 00:16:34 GMT  
		Size: 105.8 KB (105750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9bd960b18352a35d0e3621b0b93bf30fe6a4af0e6f3b3ee320a0066ab1fd6e`  
		Last Modified: Tue, 17 Dec 2019 00:16:49 GMT  
		Size: 41.7 MB (41714866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346fcafff6d4d08692fb7d8093db676fa14fe6580b7dc9f988f88d1fac9a55c3`  
		Last Modified: Tue, 17 Dec 2019 00:16:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing`

```console
$ docker pull ros@sha256:143837fc0e3190a1f94d0dfb9e892ea254eb4f295eaeaaa0847cdbfd21b139ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing` - linux; amd64

```console
$ docker pull ros@sha256:5b93920edef98f2fa1edeebdb58c0f367caaf1c05992da804728e29fe28df71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283375385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57bf406d338f7f968c56becd4dcfb5788aa6bfb16f78b555b7fefe166fc3146`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:51:30 GMT
ENV ROS_DISTRO=dashing
# Mon, 16 Dec 2019 23:27:29 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:27:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:27:30 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:27:48 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550351309565feb4d5136bc555e829b6cfb9f6793b2b6e71619ef633febc5093`  
		Last Modified: Mon, 16 Dec 2019 23:30:00 GMT  
		Size: 70.5 MB (70544098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e2b990f8ee55471cd6fca16b0a84148b742c69861080a7e292277ba1ebde1b`  
		Last Modified: Mon, 16 Dec 2019 23:29:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c64a51335a7c65157da4ae205836a05291276a04896b1867b1439ff540d3f31`  
		Last Modified: Mon, 16 Dec 2019 23:30:06 GMT  
		Size: 4.3 MB (4340407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm variant v7

```console
$ docker pull ros@sha256:bfc2aa05fd6b1eb89f67a11be7bdd8cc75d052c124cbbcd7a0b50b8bea5533b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235718036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7665ecb58e283e2011077f31a62104c8046a36660fd369c05ecd0382db4793a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Fri, 13 Dec 2019 23:08:14 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:32:16 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:32:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:32:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:32:53 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:34:05 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7771d78244221866a488a02719781d4a8900fde4615b59d77d0f8bd2dd83a2b5`  
		Last Modified: Tue, 17 Dec 2019 00:47:39 GMT  
		Size: 49.8 MB (49750290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410f3f381e447065a8b7fd3b6fef55ca5ac04280080cd19162b98940569b7d`  
		Last Modified: Tue, 17 Dec 2019 00:47:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515a2b0fd69a882073e265f4709db48c4ac07311ad179325379bffc133a9a2ee`  
		Last Modified: Tue, 17 Dec 2019 00:47:50 GMT  
		Size: 3.3 MB (3278928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4252a0d2433f8d5ba9038e782e096bbbcdcaeef4a936f417ea051f3940b7178
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210962407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f456262b7202fd3d72999d77068ac9e8743b93aa8033a1a6af1beaa4409055a9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:46:31 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:12:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:12:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:12:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:12:31 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:13:21 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89890285756a28fe746665db1a366e80da79c235768d7f9cd6c82788ff772c4a`  
		Last Modified: Tue, 17 Dec 2019 00:17:34 GMT  
		Size: 57.7 MB (57719741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de0a382654c3f46b334aa3dd3903b7d382eecec3b4ee1b907f638370aed1a6`  
		Last Modified: Tue, 17 Dec 2019 00:17:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c188498e859c14ca6f1a8f71afa133565e264495948ad383abe21b7f2865e453`  
		Last Modified: Tue, 17 Dec 2019 00:17:44 GMT  
		Size: 3.7 MB (3692825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base`

```console
$ docker pull ros@sha256:143837fc0e3190a1f94d0dfb9e892ea254eb4f295eaeaaa0847cdbfd21b139ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:5b93920edef98f2fa1edeebdb58c0f367caaf1c05992da804728e29fe28df71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283375385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57bf406d338f7f968c56becd4dcfb5788aa6bfb16f78b555b7fefe166fc3146`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:51:30 GMT
ENV ROS_DISTRO=dashing
# Mon, 16 Dec 2019 23:27:29 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:27:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:27:30 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:27:48 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550351309565feb4d5136bc555e829b6cfb9f6793b2b6e71619ef633febc5093`  
		Last Modified: Mon, 16 Dec 2019 23:30:00 GMT  
		Size: 70.5 MB (70544098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e2b990f8ee55471cd6fca16b0a84148b742c69861080a7e292277ba1ebde1b`  
		Last Modified: Mon, 16 Dec 2019 23:29:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c64a51335a7c65157da4ae205836a05291276a04896b1867b1439ff540d3f31`  
		Last Modified: Mon, 16 Dec 2019 23:30:06 GMT  
		Size: 4.3 MB (4340407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:bfc2aa05fd6b1eb89f67a11be7bdd8cc75d052c124cbbcd7a0b50b8bea5533b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235718036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7665ecb58e283e2011077f31a62104c8046a36660fd369c05ecd0382db4793a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Fri, 13 Dec 2019 23:08:14 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:32:16 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:32:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:32:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:32:53 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:34:05 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7771d78244221866a488a02719781d4a8900fde4615b59d77d0f8bd2dd83a2b5`  
		Last Modified: Tue, 17 Dec 2019 00:47:39 GMT  
		Size: 49.8 MB (49750290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410f3f381e447065a8b7fd3b6fef55ca5ac04280080cd19162b98940569b7d`  
		Last Modified: Tue, 17 Dec 2019 00:47:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515a2b0fd69a882073e265f4709db48c4ac07311ad179325379bffc133a9a2ee`  
		Last Modified: Tue, 17 Dec 2019 00:47:50 GMT  
		Size: 3.3 MB (3278928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4252a0d2433f8d5ba9038e782e096bbbcdcaeef4a936f417ea051f3940b7178
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210962407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f456262b7202fd3d72999d77068ac9e8743b93aa8033a1a6af1beaa4409055a9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:46:31 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:12:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:12:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:12:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:12:31 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:13:21 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89890285756a28fe746665db1a366e80da79c235768d7f9cd6c82788ff772c4a`  
		Last Modified: Tue, 17 Dec 2019 00:17:34 GMT  
		Size: 57.7 MB (57719741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de0a382654c3f46b334aa3dd3903b7d382eecec3b4ee1b907f638370aed1a6`  
		Last Modified: Tue, 17 Dec 2019 00:17:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c188498e859c14ca6f1a8f71afa133565e264495948ad383abe21b7f2865e453`  
		Last Modified: Tue, 17 Dec 2019 00:17:44 GMT  
		Size: 3.7 MB (3692825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base-bionic`

```console
$ docker pull ros@sha256:143837fc0e3190a1f94d0dfb9e892ea254eb4f295eaeaaa0847cdbfd21b139ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:5b93920edef98f2fa1edeebdb58c0f367caaf1c05992da804728e29fe28df71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283375385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57bf406d338f7f968c56becd4dcfb5788aa6bfb16f78b555b7fefe166fc3146`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:51:30 GMT
ENV ROS_DISTRO=dashing
# Mon, 16 Dec 2019 23:27:29 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:27:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:27:30 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:27:48 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550351309565feb4d5136bc555e829b6cfb9f6793b2b6e71619ef633febc5093`  
		Last Modified: Mon, 16 Dec 2019 23:30:00 GMT  
		Size: 70.5 MB (70544098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e2b990f8ee55471cd6fca16b0a84148b742c69861080a7e292277ba1ebde1b`  
		Last Modified: Mon, 16 Dec 2019 23:29:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c64a51335a7c65157da4ae205836a05291276a04896b1867b1439ff540d3f31`  
		Last Modified: Mon, 16 Dec 2019 23:30:06 GMT  
		Size: 4.3 MB (4340407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:bfc2aa05fd6b1eb89f67a11be7bdd8cc75d052c124cbbcd7a0b50b8bea5533b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235718036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7665ecb58e283e2011077f31a62104c8046a36660fd369c05ecd0382db4793a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Fri, 13 Dec 2019 23:08:14 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:32:16 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:32:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:32:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:32:53 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:34:05 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7771d78244221866a488a02719781d4a8900fde4615b59d77d0f8bd2dd83a2b5`  
		Last Modified: Tue, 17 Dec 2019 00:47:39 GMT  
		Size: 49.8 MB (49750290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410f3f381e447065a8b7fd3b6fef55ca5ac04280080cd19162b98940569b7d`  
		Last Modified: Tue, 17 Dec 2019 00:47:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515a2b0fd69a882073e265f4709db48c4ac07311ad179325379bffc133a9a2ee`  
		Last Modified: Tue, 17 Dec 2019 00:47:50 GMT  
		Size: 3.3 MB (3278928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4252a0d2433f8d5ba9038e782e096bbbcdcaeef4a936f417ea051f3940b7178
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210962407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f456262b7202fd3d72999d77068ac9e8743b93aa8033a1a6af1beaa4409055a9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:46:31 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:12:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:12:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:12:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:12:31 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:13:21 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89890285756a28fe746665db1a366e80da79c235768d7f9cd6c82788ff772c4a`  
		Last Modified: Tue, 17 Dec 2019 00:17:34 GMT  
		Size: 57.7 MB (57719741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de0a382654c3f46b334aa3dd3903b7d382eecec3b4ee1b907f638370aed1a6`  
		Last Modified: Tue, 17 Dec 2019 00:17:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c188498e859c14ca6f1a8f71afa133565e264495948ad383abe21b7f2865e453`  
		Last Modified: Tue, 17 Dec 2019 00:17:44 GMT  
		Size: 3.7 MB (3692825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core`

```console
$ docker pull ros@sha256:d1b117a3768bb6ce8d42c25073faf0ba226277334a7cf605e3278671c8d57f41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:78896289b15b410d1dfa3627e8add8b38308b2e12a537de875f315bb6c2889fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.0 MB (279034978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1ab6b0eed99e368663da2fa8ba7f3a2a3bfaa4aab18ed01af039e66d2d5c44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:51:30 GMT
ENV ROS_DISTRO=dashing
# Mon, 16 Dec 2019 23:27:29 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:27:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:27:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550351309565feb4d5136bc555e829b6cfb9f6793b2b6e71619ef633febc5093`  
		Last Modified: Mon, 16 Dec 2019 23:30:00 GMT  
		Size: 70.5 MB (70544098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e2b990f8ee55471cd6fca16b0a84148b742c69861080a7e292277ba1ebde1b`  
		Last Modified: Mon, 16 Dec 2019 23:29:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:8de646f1e2e99e658b20dc66e77442ebe7b3ac55a63eec22bd4c310c46102293
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232439108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6afb9bbb42acdcdb5fd33eae5fad60cc783a583eab9ddffaaf71301be398729`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Fri, 13 Dec 2019 23:08:14 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:32:16 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:32:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:32:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:32:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7771d78244221866a488a02719781d4a8900fde4615b59d77d0f8bd2dd83a2b5`  
		Last Modified: Tue, 17 Dec 2019 00:47:39 GMT  
		Size: 49.8 MB (49750290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410f3f381e447065a8b7fd3b6fef55ca5ac04280080cd19162b98940569b7d`  
		Last Modified: Tue, 17 Dec 2019 00:47:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bdbece47d96fd98cfc4da79113cccd0c92d9187dc55fe9bde177ca62ee260c50
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.3 MB (207269582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be092a3a5d598582873db3738dcd517f57d00bdfb46d9f08a11155554c59348`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:46:31 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:12:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:12:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:12:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:12:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89890285756a28fe746665db1a366e80da79c235768d7f9cd6c82788ff772c4a`  
		Last Modified: Tue, 17 Dec 2019 00:17:34 GMT  
		Size: 57.7 MB (57719741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de0a382654c3f46b334aa3dd3903b7d382eecec3b4ee1b907f638370aed1a6`  
		Last Modified: Tue, 17 Dec 2019 00:17:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core-bionic`

```console
$ docker pull ros@sha256:d1b117a3768bb6ce8d42c25073faf0ba226277334a7cf605e3278671c8d57f41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:78896289b15b410d1dfa3627e8add8b38308b2e12a537de875f315bb6c2889fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.0 MB (279034978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1ab6b0eed99e368663da2fa8ba7f3a2a3bfaa4aab18ed01af039e66d2d5c44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:51:30 GMT
ENV ROS_DISTRO=dashing
# Mon, 16 Dec 2019 23:27:29 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:27:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:27:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550351309565feb4d5136bc555e829b6cfb9f6793b2b6e71619ef633febc5093`  
		Last Modified: Mon, 16 Dec 2019 23:30:00 GMT  
		Size: 70.5 MB (70544098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e2b990f8ee55471cd6fca16b0a84148b742c69861080a7e292277ba1ebde1b`  
		Last Modified: Mon, 16 Dec 2019 23:29:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:8de646f1e2e99e658b20dc66e77442ebe7b3ac55a63eec22bd4c310c46102293
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232439108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6afb9bbb42acdcdb5fd33eae5fad60cc783a583eab9ddffaaf71301be398729`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Fri, 13 Dec 2019 23:08:14 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:32:16 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:32:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:32:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:32:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7771d78244221866a488a02719781d4a8900fde4615b59d77d0f8bd2dd83a2b5`  
		Last Modified: Tue, 17 Dec 2019 00:47:39 GMT  
		Size: 49.8 MB (49750290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410f3f381e447065a8b7fd3b6fef55ca5ac04280080cd19162b98940569b7d`  
		Last Modified: Tue, 17 Dec 2019 00:47:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bdbece47d96fd98cfc4da79113cccd0c92d9187dc55fe9bde177ca62ee260c50
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.3 MB (207269582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be092a3a5d598582873db3738dcd517f57d00bdfb46d9f08a11155554c59348`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Thu, 31 Oct 2019 23:46:31 GMT
ENV ROS_DISTRO=dashing
# Tue, 17 Dec 2019 00:12:20 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:12:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:12:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:12:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89890285756a28fe746665db1a366e80da79c235768d7f9cd6c82788ff772c4a`  
		Last Modified: Tue, 17 Dec 2019 00:17:34 GMT  
		Size: 57.7 MB (57719741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de0a382654c3f46b334aa3dd3903b7d382eecec3b4ee1b907f638370aed1a6`  
		Last Modified: Tue, 17 Dec 2019 00:17:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent`

```console
$ docker pull ros@sha256:4ee7671bdf6856ec75cd7e667fef0465fb697b0700b1423e929dd9a816793d8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent` - linux; amd64

```console
$ docker pull ros@sha256:ac136d6885b3829e7f9c7d6348f7c6db14bb9faadc5ff1d7acf2a1c0a9e690dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285608882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544b7f9ea521869846affd04190de7fd9d9911fe9c4c18f699eed4381ee5f5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:22:52 GMT
ENV ROS_DISTRO=eloquent
# Mon, 16 Dec 2019 23:28:32 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:28:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:28:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:28:33 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:28:45 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97089b92da5d6c8325e36b447e3114d61451d0b7d60d1396ee00554852a021f`  
		Last Modified: Mon, 16 Dec 2019 23:30:27 GMT  
		Size: 72.5 MB (72516550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c3fa76c8ca8d9bea99348f725852362fbb4e29ad2149e34e130a968237a2e`  
		Last Modified: Mon, 16 Dec 2019 23:30:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f71a06296ea89714cdb4b3f42e8678e8361d815bdf50c7debe535cd775a754b`  
		Last Modified: Mon, 16 Dec 2019 23:30:32 GMT  
		Size: 4.6 MB (4601452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm variant v7

```console
$ docker pull ros@sha256:91209b5d039b9ef461180799d58c472cb8d0f60e02ebd4f6b4fdc7dc4d3f3dc0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237553860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e4b3eec2d3a2c3939ee981d909e668dcff0a7d9dff53ef57b4794ec7222c91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Thu, 28 Nov 2019 00:03:51 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:44:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:44:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:44:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:45:03 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:46:34 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e768833718921e59f9bffa739072eb04563e70bdc8a8f6c954140c6c0a3852`  
		Last Modified: Tue, 17 Dec 2019 00:48:24 GMT  
		Size: 51.3 MB (51347905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77d0cd346635b5a0aed6978239261fc78592fe0b2c5b6e7f04b6f2363ce2e8c`  
		Last Modified: Tue, 17 Dec 2019 00:48:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0537751595c692d538988cb48b37b386a7e7d11556aa78db10ad4f76af731f97`  
		Last Modified: Tue, 17 Dec 2019 00:48:37 GMT  
		Size: 3.5 MB (3517137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:acb2eb39ba95187065da0f8d9815604d9b5a3f3c2c7a82e1a855a99001142a1d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.1 MB (213074956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09bda8b8d751e32a08d081c9055339382b11c0d6a84078bda8cc2597b7ef16e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:41:14 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:15:07 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:15:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:15:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:15:12 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:15:56 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9d6629452340db008836d42f5140006c663d5520c43e95e88f74d3808b4fe8`  
		Last Modified: Tue, 17 Dec 2019 00:18:21 GMT  
		Size: 59.6 MB (59571626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174f5f0816548b73561472df3e00def59a47185f6176dc935a432b7a40986004`  
		Last Modified: Tue, 17 Dec 2019 00:17:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8fc85c769167d3d3a0e7b0e82e3b754d23931e5e231593ee2f562fb9ecd508`  
		Last Modified: Tue, 17 Dec 2019 00:18:47 GMT  
		Size: 4.0 MB (3953490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-base`

```console
$ docker pull ros@sha256:4ee7671bdf6856ec75cd7e667fef0465fb697b0700b1423e929dd9a816793d8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:ac136d6885b3829e7f9c7d6348f7c6db14bb9faadc5ff1d7acf2a1c0a9e690dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285608882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544b7f9ea521869846affd04190de7fd9d9911fe9c4c18f699eed4381ee5f5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:22:52 GMT
ENV ROS_DISTRO=eloquent
# Mon, 16 Dec 2019 23:28:32 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:28:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:28:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:28:33 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:28:45 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97089b92da5d6c8325e36b447e3114d61451d0b7d60d1396ee00554852a021f`  
		Last Modified: Mon, 16 Dec 2019 23:30:27 GMT  
		Size: 72.5 MB (72516550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c3fa76c8ca8d9bea99348f725852362fbb4e29ad2149e34e130a968237a2e`  
		Last Modified: Mon, 16 Dec 2019 23:30:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f71a06296ea89714cdb4b3f42e8678e8361d815bdf50c7debe535cd775a754b`  
		Last Modified: Mon, 16 Dec 2019 23:30:32 GMT  
		Size: 4.6 MB (4601452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:91209b5d039b9ef461180799d58c472cb8d0f60e02ebd4f6b4fdc7dc4d3f3dc0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237553860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e4b3eec2d3a2c3939ee981d909e668dcff0a7d9dff53ef57b4794ec7222c91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Thu, 28 Nov 2019 00:03:51 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:44:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:44:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:44:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:45:03 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:46:34 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e768833718921e59f9bffa739072eb04563e70bdc8a8f6c954140c6c0a3852`  
		Last Modified: Tue, 17 Dec 2019 00:48:24 GMT  
		Size: 51.3 MB (51347905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77d0cd346635b5a0aed6978239261fc78592fe0b2c5b6e7f04b6f2363ce2e8c`  
		Last Modified: Tue, 17 Dec 2019 00:48:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0537751595c692d538988cb48b37b386a7e7d11556aa78db10ad4f76af731f97`  
		Last Modified: Tue, 17 Dec 2019 00:48:37 GMT  
		Size: 3.5 MB (3517137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:acb2eb39ba95187065da0f8d9815604d9b5a3f3c2c7a82e1a855a99001142a1d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.1 MB (213074956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09bda8b8d751e32a08d081c9055339382b11c0d6a84078bda8cc2597b7ef16e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:41:14 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:15:07 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:15:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:15:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:15:12 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:15:56 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9d6629452340db008836d42f5140006c663d5520c43e95e88f74d3808b4fe8`  
		Last Modified: Tue, 17 Dec 2019 00:18:21 GMT  
		Size: 59.6 MB (59571626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174f5f0816548b73561472df3e00def59a47185f6176dc935a432b7a40986004`  
		Last Modified: Tue, 17 Dec 2019 00:17:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8fc85c769167d3d3a0e7b0e82e3b754d23931e5e231593ee2f562fb9ecd508`  
		Last Modified: Tue, 17 Dec 2019 00:18:47 GMT  
		Size: 4.0 MB (3953490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-base-bionic`

```console
$ docker pull ros@sha256:4ee7671bdf6856ec75cd7e667fef0465fb697b0700b1423e929dd9a816793d8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:ac136d6885b3829e7f9c7d6348f7c6db14bb9faadc5ff1d7acf2a1c0a9e690dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285608882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544b7f9ea521869846affd04190de7fd9d9911fe9c4c18f699eed4381ee5f5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:22:52 GMT
ENV ROS_DISTRO=eloquent
# Mon, 16 Dec 2019 23:28:32 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:28:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:28:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:28:33 GMT
CMD ["bash"]
# Mon, 16 Dec 2019 23:28:45 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97089b92da5d6c8325e36b447e3114d61451d0b7d60d1396ee00554852a021f`  
		Last Modified: Mon, 16 Dec 2019 23:30:27 GMT  
		Size: 72.5 MB (72516550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c3fa76c8ca8d9bea99348f725852362fbb4e29ad2149e34e130a968237a2e`  
		Last Modified: Mon, 16 Dec 2019 23:30:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f71a06296ea89714cdb4b3f42e8678e8361d815bdf50c7debe535cd775a754b`  
		Last Modified: Mon, 16 Dec 2019 23:30:32 GMT  
		Size: 4.6 MB (4601452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:91209b5d039b9ef461180799d58c472cb8d0f60e02ebd4f6b4fdc7dc4d3f3dc0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237553860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e4b3eec2d3a2c3939ee981d909e668dcff0a7d9dff53ef57b4794ec7222c91`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Thu, 28 Nov 2019 00:03:51 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:44:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:44:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:44:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:45:03 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:46:34 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e768833718921e59f9bffa739072eb04563e70bdc8a8f6c954140c6c0a3852`  
		Last Modified: Tue, 17 Dec 2019 00:48:24 GMT  
		Size: 51.3 MB (51347905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77d0cd346635b5a0aed6978239261fc78592fe0b2c5b6e7f04b6f2363ce2e8c`  
		Last Modified: Tue, 17 Dec 2019 00:48:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0537751595c692d538988cb48b37b386a7e7d11556aa78db10ad4f76af731f97`  
		Last Modified: Tue, 17 Dec 2019 00:48:37 GMT  
		Size: 3.5 MB (3517137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:acb2eb39ba95187065da0f8d9815604d9b5a3f3c2c7a82e1a855a99001142a1d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.1 MB (213074956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09bda8b8d751e32a08d081c9055339382b11c0d6a84078bda8cc2597b7ef16e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:41:14 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:15:07 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:15:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:15:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:15:12 GMT
CMD ["bash"]
# Tue, 17 Dec 2019 00:15:56 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9d6629452340db008836d42f5140006c663d5520c43e95e88f74d3808b4fe8`  
		Last Modified: Tue, 17 Dec 2019 00:18:21 GMT  
		Size: 59.6 MB (59571626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174f5f0816548b73561472df3e00def59a47185f6176dc935a432b7a40986004`  
		Last Modified: Tue, 17 Dec 2019 00:17:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8fc85c769167d3d3a0e7b0e82e3b754d23931e5e231593ee2f562fb9ecd508`  
		Last Modified: Tue, 17 Dec 2019 00:18:47 GMT  
		Size: 4.0 MB (3953490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-core`

```console
$ docker pull ros@sha256:4a743f9565dda444c3b05e85e90d5e3ec633a189494153113772bce5b65567f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5b75f45cc30275f491428a81ad158434ec950f68c594fd4f0e2e1743060c5c95
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (281007430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ad32ec40d94be0d64ec2fa6261b306772e68fb32ffa07a4c32e648a6ccd636`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:22:52 GMT
ENV ROS_DISTRO=eloquent
# Mon, 16 Dec 2019 23:28:32 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:28:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:28:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:28:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97089b92da5d6c8325e36b447e3114d61451d0b7d60d1396ee00554852a021f`  
		Last Modified: Mon, 16 Dec 2019 23:30:27 GMT  
		Size: 72.5 MB (72516550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c3fa76c8ca8d9bea99348f725852362fbb4e29ad2149e34e130a968237a2e`  
		Last Modified: Mon, 16 Dec 2019 23:30:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:8039a684163f44d525a702092d4fd3e730ee96cc62483428f778e786d52255b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (234036723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:024504a796375bac4fce05da17883748744deb63127b20aea76f0fb9a14d82dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Thu, 28 Nov 2019 00:03:51 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:44:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:44:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:44:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:45:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e768833718921e59f9bffa739072eb04563e70bdc8a8f6c954140c6c0a3852`  
		Last Modified: Tue, 17 Dec 2019 00:48:24 GMT  
		Size: 51.3 MB (51347905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77d0cd346635b5a0aed6978239261fc78592fe0b2c5b6e7f04b6f2363ce2e8c`  
		Last Modified: Tue, 17 Dec 2019 00:48:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5f2b85f0b2e16f118507aeed7cc74a9603ef27fee033ad77e64b4bfff9a744a6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.1 MB (209121466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6f5b9f72db6f849bc5eba2ff18b8c6ef376e1b647acc74325bc1e1323b3163`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:41:14 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:15:07 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:15:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:15:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:15:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9d6629452340db008836d42f5140006c663d5520c43e95e88f74d3808b4fe8`  
		Last Modified: Tue, 17 Dec 2019 00:18:21 GMT  
		Size: 59.6 MB (59571626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174f5f0816548b73561472df3e00def59a47185f6176dc935a432b7a40986004`  
		Last Modified: Tue, 17 Dec 2019 00:17:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-core-bionic`

```console
$ docker pull ros@sha256:4a743f9565dda444c3b05e85e90d5e3ec633a189494153113772bce5b65567f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:5b75f45cc30275f491428a81ad158434ec950f68c594fd4f0e2e1743060c5c95
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (281007430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ad32ec40d94be0d64ec2fa6261b306772e68fb32ffa07a4c32e648a6ccd636`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:32 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:49:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:50:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:50:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:50:20 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:50:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:50:25 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:22:52 GMT
ENV ROS_DISTRO=eloquent
# Mon, 16 Dec 2019 23:28:32 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Dec 2019 23:28:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 16 Dec 2019 23:28:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 16 Dec 2019 23:28:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbeaf2264163bd4a00c0f88a59e883c1ee63fec393bc29c53389deeeb753569`  
		Last Modified: Fri, 01 Nov 2019 00:00:08 GMT  
		Size: 152.0 MB (152005276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa38d9f2eb3f3f2cce1a4c0bdd7cb51bba9fb9a80f1a8701f8f884a5a2558c0`  
		Last Modified: Thu, 31 Oct 2019 23:59:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7b74aa34f7ee2627ab68377ebc7b664454d2698690bd7375e128aae3f4922`  
		Last Modified: Thu, 31 Oct 2019 23:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f6d25756e51299201ad02a29bb1bf7854a68d8ee816a4cf7da12b57ae7ce13`  
		Last Modified: Thu, 31 Oct 2019 23:59:47 GMT  
		Size: 28.4 MB (28384356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3889cab82ec0e1bdaf9cc2b87521e35b2aa1aaca255c365f162063f42a289f`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 440.1 KB (440052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b344d6fdfa49d8debc776d6dfc5b8e861c5623fe775e3e1db9c8b1b08f804a`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 1.9 KB (1898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5bb9cf1f52be160ccceaa18b01924f8fb02ec488f4978875c745f75e381184`  
		Last Modified: Thu, 31 Oct 2019 23:59:37 GMT  
		Size: 94.9 KB (94909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97089b92da5d6c8325e36b447e3114d61451d0b7d60d1396ee00554852a021f`  
		Last Modified: Mon, 16 Dec 2019 23:30:27 GMT  
		Size: 72.5 MB (72516550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c3fa76c8ca8d9bea99348f725852362fbb4e29ad2149e34e130a968237a2e`  
		Last Modified: Mon, 16 Dec 2019 23:30:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:8039a684163f44d525a702092d4fd3e730ee96cc62483428f778e786d52255b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (234036723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:024504a796375bac4fce05da17883748744deb63127b20aea76f0fb9a14d82dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:13 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:02:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 28 Nov 2019 00:02:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 28 Nov 2019 00:03:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Nov 2019 00:03:22 GMT
ENV LANG=C.UTF-8
# Thu, 28 Nov 2019 00:03:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 28 Nov 2019 00:03:42 GMT
RUN rosdep init     && rosdep update
# Thu, 28 Nov 2019 00:03:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 28 Nov 2019 00:03:51 GMT
RUN pip3 install -U     argcomplete
# Thu, 28 Nov 2019 00:03:51 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:44:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:44:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:44:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:45:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67eb6c552df64a42abac769ad84f5426eaccc2c31f4b8d25c89fd37d0999e8`  
		Last Modified: Thu, 28 Nov 2019 00:06:57 GMT  
		Size: 133.6 MB (133619890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5485052daf7b051e1e4073f845dc54955242f7a204af771d58d5c8a20fea22fd`  
		Last Modified: Thu, 28 Nov 2019 00:06:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ba7e40c4635262b019089d9bfd455c8bfe464ac9feb70de8c1c23aa88eb7f`  
		Last Modified: Thu, 28 Nov 2019 00:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0bde61a23326e9b53f0d5ce32511c314d86d672e27e7df55d3cfec9f7482c`  
		Last Modified: Thu, 28 Nov 2019 00:06:29 GMT  
		Size: 25.4 MB (25359176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e0847e6cec425dee1c16d1f59618ed011d936863e389fa19cfadee535dc3`  
		Last Modified: Thu, 28 Nov 2019 00:06:20 GMT  
		Size: 450.9 KB (450944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efa6669b86fc375af378e4c2d4e7369c87821afa37b3e77bad419777b11f9c4`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73173f02abf186cc9678da9e4037bd685e825e1624fc2fa6db2522a9ad5c7d`  
		Last Modified: Thu, 28 Nov 2019 00:06:19 GMT  
		Size: 105.7 KB (105735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e768833718921e59f9bffa739072eb04563e70bdc8a8f6c954140c6c0a3852`  
		Last Modified: Tue, 17 Dec 2019 00:48:24 GMT  
		Size: 51.3 MB (51347905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77d0cd346635b5a0aed6978239261fc78592fe0b2c5b6e7f04b6f2363ce2e8c`  
		Last Modified: Tue, 17 Dec 2019 00:48:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5f2b85f0b2e16f118507aeed7cc74a9603ef27fee033ad77e64b4bfff9a744a6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.1 MB (209121466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6f5b9f72db6f849bc5eba2ff18b8c6ef376e1b647acc74325bc1e1323b3163`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:42:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 31 Oct 2019 23:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:43:50 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:43:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:44:13 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:44:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 31 Oct 2019 23:44:24 GMT
RUN pip3 install -U     argcomplete
# Wed, 27 Nov 2019 23:41:14 GMT
ENV ROS_DISTRO=eloquent
# Tue, 17 Dec 2019 00:15:07 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Dec 2019 00:15:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 17 Dec 2019 00:15:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Dec 2019 00:15:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9569ff9543878cd5daf8d1c9eba5d48688b763d4d7a4950ed5831eb33cf6c`  
		Last Modified: Thu, 31 Oct 2019 23:57:48 GMT  
		Size: 97.4 MB (97352390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5503d0031d4c62f5b8455f91ea9869d90564d02e8a934faac1d1f8be0e59d`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2185d293e7101e0321dc0e2d6fbb44eda3a4cb5d9a7d055ee7850be069ba3`  
		Last Modified: Thu, 31 Oct 2019 23:57:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb400b2c833f2a509f7a6a07b9fcf7c8e6fafd0380634c23dfcf53a44de450`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 27.1 MB (27066077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c65f811146f773b9460df37d0dd9f5b4064f870e12978c2088b6643e8c5b4`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 440.1 KB (440108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff905670d8fb02b2bd65d0e2ad4e70aba998f4401d7b0257f87a4d2c5898050`  
		Last Modified: Thu, 31 Oct 2019 23:57:14 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f9d3d8cbfa41b7a51a67fbb059349049c3befcfc58a4de47204036aaf916de`  
		Last Modified: Thu, 31 Oct 2019 23:57:15 GMT  
		Size: 95.0 KB (95038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9d6629452340db008836d42f5140006c663d5520c43e95e88f74d3808b4fe8`  
		Last Modified: Tue, 17 Dec 2019 00:18:21 GMT  
		Size: 59.6 MB (59571626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174f5f0816548b73561472df3e00def59a47185f6176dc935a432b7a40986004`  
		Last Modified: Tue, 17 Dec 2019 00:17:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic`

```console
$ docker pull ros@sha256:fa4f8c779968d89dc1ce9e3b37cfc785245bd907dfb480fc1a656df703350f61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:328ca8346b5d8366685b1061ceb959a40bf28e1db45e39b420a528c7ac7ba65d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385369213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c20092b18eddd2fcf94eebf33e24ce011760caf804eee41217f36d9067dda04`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f362444c6365d013df2de863de982a8d168027a61ea31076b9a9ba618589d5c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336676293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfdb7556519f8e867911e4b115eabd160a07ae3b6ed17e546a71f45799d9cd2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4f2d68c4c3aabc6b84fd664c9d4e1e67fefdd0ff74664f4f4def3189bd39214
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350479932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64b8b9e62ca477d70be1b352d32154f88f1388531eb28c7c6977a700d11aef5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:44ffc3d080c4d2b04356339e00174e8ca5ec2c4e6481372734eaa469eee5093a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:22de151a5463cfeddb2607395e32b9fc423f516a5fb9ff706f68618ba0ac966f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.8 MB (725803096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831f9da45e46caf70171ca24d4e75c564937bc3781e68db017b3c686683b9d09`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:29:55 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839962451fef702e5a136881d47c3e88c82e57dba46f61223c1737bc11ea6b9`  
		Last Modified: Wed, 27 Nov 2019 01:33:46 GMT  
		Size: 340.4 MB (340433883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:9350725e5154518df02a58b8e7e494aa998f80e42a7ae2e4db30a2ed0c4ba504
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.2 MB (617162994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219d84e545ecf8c12df92730af542f02a7bfe5f9dec7f61b5a4735a1416bef11`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:06:28 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4000e1a9649e8da11f7bf75af1351eed54464e26d6ea290ca1f8a470602ba2a0`  
		Last Modified: Wed, 27 Nov 2019 01:10:57 GMT  
		Size: 280.5 MB (280486701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6104958cbb00f5134618b1b5ac7723ec1679d9e98aef8c507afea6aae34cdc6b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.4 MB (641442869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03e9e79f5ac21e8693f454646f82e56434d383ba8731c7462694c447ef7331f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:24:47 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c7219a65d4acec5d6f8e0dbc20ecab05786968bc8b816e33f018952770853f`  
		Last Modified: Wed, 27 Nov 2019 00:29:54 GMT  
		Size: 291.0 MB (290962937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:44ffc3d080c4d2b04356339e00174e8ca5ec2c4e6481372734eaa469eee5093a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:22de151a5463cfeddb2607395e32b9fc423f516a5fb9ff706f68618ba0ac966f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.8 MB (725803096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831f9da45e46caf70171ca24d4e75c564937bc3781e68db017b3c686683b9d09`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:29:55 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1839962451fef702e5a136881d47c3e88c82e57dba46f61223c1737bc11ea6b9`  
		Last Modified: Wed, 27 Nov 2019 01:33:46 GMT  
		Size: 340.4 MB (340433883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:9350725e5154518df02a58b8e7e494aa998f80e42a7ae2e4db30a2ed0c4ba504
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.2 MB (617162994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219d84e545ecf8c12df92730af542f02a7bfe5f9dec7f61b5a4735a1416bef11`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:06:28 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4000e1a9649e8da11f7bf75af1351eed54464e26d6ea290ca1f8a470602ba2a0`  
		Last Modified: Wed, 27 Nov 2019 01:10:57 GMT  
		Size: 280.5 MB (280486701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6104958cbb00f5134618b1b5ac7723ec1679d9e98aef8c507afea6aae34cdc6b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.4 MB (641442869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03e9e79f5ac21e8693f454646f82e56434d383ba8731c7462694c447ef7331f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:24:47 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c7219a65d4acec5d6f8e0dbc20ecab05786968bc8b816e33f018952770853f`  
		Last Modified: Wed, 27 Nov 2019 00:29:54 GMT  
		Size: 291.0 MB (290962937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:b2a26c119a9f1bff6ad489b765d5bde2c15528077f860f3a63d4a0eebd0f6688
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:4179e9d545eeb24258795b19ca25c1636e76ad4148dde5b346ad88fa78c5a380
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.0 MB (489005885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e556b557365575030ddafb7904f3bed4be9baa54ca836f8dd0b4bd7f29ccf47`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:27:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf67d81b3a8961de514e9a889df80b430726479fca6c7f7e5bbcce7066e93bc9`  
		Last Modified: Wed, 27 Nov 2019 01:32:36 GMT  
		Size: 103.6 MB (103636672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:f14d33f678d0f0a3f8937992ae08a67551ab1d2118c282589ed836d92eeeb8a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.7 MB (426716353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f539143e06a8fa2db495f2eae4c5104dd8465534b2fb2f7c666a8174f477f29e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:58:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86623388e10873110589506b40b66c0ad7968990fb07426054b449ac2003de`  
		Last Modified: Wed, 27 Nov 2019 01:09:22 GMT  
		Size: 90.0 MB (90040060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:85f01521d83a0559df50ead0a181726a63969e78cfe900abcaae3d94650f523c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.4 MB (444397894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8dbf2cd7f0e3b28fd29f220e856c56ebf5d8ac9535400a4d6e8c3ae2ce4ac0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:20:53 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26811bc2a2936f39aae401d4445d16251fbd32b508840ea1e64bce79ef9ff9`  
		Last Modified: Wed, 27 Nov 2019 00:28:16 GMT  
		Size: 93.9 MB (93917962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:b2a26c119a9f1bff6ad489b765d5bde2c15528077f860f3a63d4a0eebd0f6688
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:4179e9d545eeb24258795b19ca25c1636e76ad4148dde5b346ad88fa78c5a380
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.0 MB (489005885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e556b557365575030ddafb7904f3bed4be9baa54ca836f8dd0b4bd7f29ccf47`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:27:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf67d81b3a8961de514e9a889df80b430726479fca6c7f7e5bbcce7066e93bc9`  
		Last Modified: Wed, 27 Nov 2019 01:32:36 GMT  
		Size: 103.6 MB (103636672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:f14d33f678d0f0a3f8937992ae08a67551ab1d2118c282589ed836d92eeeb8a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.7 MB (426716353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f539143e06a8fa2db495f2eae4c5104dd8465534b2fb2f7c666a8174f477f29e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:58:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86623388e10873110589506b40b66c0ad7968990fb07426054b449ac2003de`  
		Last Modified: Wed, 27 Nov 2019 01:09:22 GMT  
		Size: 90.0 MB (90040060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:85f01521d83a0559df50ead0a181726a63969e78cfe900abcaae3d94650f523c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.4 MB (444397894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8dbf2cd7f0e3b28fd29f220e856c56ebf5d8ac9535400a4d6e8c3ae2ce4ac0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:20:53 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26811bc2a2936f39aae401d4445d16251fbd32b508840ea1e64bce79ef9ff9`  
		Last Modified: Wed, 27 Nov 2019 00:28:16 GMT  
		Size: 93.9 MB (93917962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:fa4f8c779968d89dc1ce9e3b37cfc785245bd907dfb480fc1a656df703350f61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:328ca8346b5d8366685b1061ceb959a40bf28e1db45e39b420a528c7ac7ba65d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385369213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c20092b18eddd2fcf94eebf33e24ce011760caf804eee41217f36d9067dda04`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:f362444c6365d013df2de863de982a8d168027a61ea31076b9a9ba618589d5c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336676293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfdb7556519f8e867911e4b115eabd160a07ae3b6ed17e546a71f45799d9cd2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4f2d68c4c3aabc6b84fd664c9d4e1e67fefdd0ff74664f4f4def3189bd39214
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350479932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64b8b9e62ca477d70be1b352d32154f88f1388531eb28c7c6977a700d11aef5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:fa4f8c779968d89dc1ce9e3b37cfc785245bd907dfb480fc1a656df703350f61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:328ca8346b5d8366685b1061ceb959a40bf28e1db45e39b420a528c7ac7ba65d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385369213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c20092b18eddd2fcf94eebf33e24ce011760caf804eee41217f36d9067dda04`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 01:26:00 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4cee62902b4ac893136b72c59d7ddca9bd5e6ed8df55a25f49bd207cd36bb7`  
		Last Modified: Wed, 27 Nov 2019 01:32:03 GMT  
		Size: 85.5 MB (85516413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:f362444c6365d013df2de863de982a8d168027a61ea31076b9a9ba618589d5c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336676293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfdb7556519f8e867911e4b115eabd160a07ae3b6ed17e546a71f45799d9cd2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:56:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fc365150ba25919e8dbe23fc2b303914e824822f2daae3cf6211333c5b0a2`  
		Last Modified: Wed, 27 Nov 2019 01:08:43 GMT  
		Size: 76.3 MB (76328765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4f2d68c4c3aabc6b84fd664c9d4e1e67fefdd0ff74664f4f4def3189bd39214
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350479932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64b8b9e62ca477d70be1b352d32154f88f1388531eb28c7c6977a700d11aef5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
# Wed, 27 Nov 2019 00:19:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bf95fa418a228fdcdfe262d1718d24977c587c9874a7c95d0dc26f1686b63b`  
		Last Modified: Wed, 27 Nov 2019 00:27:38 GMT  
		Size: 77.8 MB (77818751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:4deccc84fb3a25fc006f101a692a2f9a8fb9cc259d387bdf6bff3beea9c1236e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:8b94c619b83c45aa328402bc97781e732a96119354665c411d99c9ee161bdf74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299852800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69f289b6d142b3ec247fcbddd15988a55c1622086d9a23b32e62425a71c9d7aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:f022de41931bf8e2f9c35ba17af08d986690e9417ad1c87c732488a6cdfe0249
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260347528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ca88c446aa597e4d6cbbf3d362c9530290b8b72b9cc5c11f3936318054c2cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed72b6ceb1eec3adc23bb617423c506edb26f3bea8156eae5447033b3a2d3b77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272661181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3beeee60a73ad8863ad10c6f73b5b667be0650daae1f3cdbb255cb7f7c903a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:4deccc84fb3a25fc006f101a692a2f9a8fb9cc259d387bdf6bff3beea9c1236e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:8b94c619b83c45aa328402bc97781e732a96119354665c411d99c9ee161bdf74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299852800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69f289b6d142b3ec247fcbddd15988a55c1622086d9a23b32e62425a71c9d7aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:22:54 GMT
ADD file:4eb02fc768cad452a37e8df30bbfcc728f3e6e7ca33af177fd4de06fd07c2098 in / 
# Wed, 27 Nov 2019 00:22:55 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:22:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:22:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:22:56 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 01:22:53 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:22:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 01:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 01:23:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 01:23:34 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 01:23:42 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 01:23:42 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 01:24:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 01:24:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 01:24:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 01:24:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:976a760c94fcdd7d105269ae621e8269e7bb25a58c52ae667b4029a6bc7e33cb`  
		Last Modified: Sat, 09 Nov 2019 00:25:10 GMT  
		Size: 44.1 MB (44145376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58992f3c37bb64aeba18910408cda9a7a63e212fe27e95065a8d54130ca5926`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca0e5e7f12e6eb512246aea5579fcb771fe7203bc60944384d5cd7962f87ddb`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a274cc00ca5f671b1740c43672dbc96504760cee585e7604029a3fe56854a8`  
		Last Modified: Wed, 27 Nov 2019 00:23:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2413f0bed0a66209ed901246e8f151ba518e4eb1b3717303e00875df171b1849`  
		Last Modified: Wed, 27 Nov 2019 01:31:00 GMT  
		Size: 6.9 MB (6937889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e0c2ce6f0e60388ac30ab3ef602ab2c5d08198ed68d3e31493eb6988e0cc5c`  
		Last Modified: Wed, 27 Nov 2019 01:30:58 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74e531bbd7e8c79e58e585334eadd9373789999db201d52c0e860943c0d3af`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9251e3530954074e36ff8e50c883310a9605499d1916764b3c822fedea5c58f3`  
		Last Modified: Wed, 27 Nov 2019 01:31:14 GMT  
		Size: 54.8 MB (54770079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff08d617d661fe4f2c1b1ae7689a76647297e9bde6b1fe2d816a0f4a0c18aa1`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 443.6 KB (443566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c1a5ab74dd08973c5069b70883e6fd13e4768aa015cd974ef8f30ef39e0179`  
		Last Modified: Wed, 27 Nov 2019 01:31:40 GMT  
		Size: 193.5 MB (193540826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94430f6a50379155ae297c72319861669ef978a8e555187a7393f78df72dc937`  
		Last Modified: Wed, 27 Nov 2019 01:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:f022de41931bf8e2f9c35ba17af08d986690e9417ad1c87c732488a6cdfe0249
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260347528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ca88c446aa597e4d6cbbf3d362c9530290b8b72b9cc5c11f3936318054c2cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 27 Nov 2019 00:18:53 GMT
ADD file:0a7e692f03565b8c1a21c3fc1763d997bf91ba1568698ff5532bbc4098fec405 in / 
# Wed, 27 Nov 2019 00:19:00 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:19:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 27 Nov 2019 00:19:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 27 Nov 2019 00:19:12 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:49:50 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:49:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:49:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:51:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:51:55 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:51:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:52:17 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:52:18 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:54:37 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:54:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:54:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:54:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e8e75463be38652e5e282a037f1fbc29fdd17fcf52a656968af73779867d9f0f`  
		Last Modified: Mon, 11 Nov 2019 15:38:43 GMT  
		Size: 38.9 MB (38881137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c095f19b697e97a3f22e2888c5a369f8b4081bc1d8dc69ea36cfd30d56aa746`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cffb842254e9bd8c3806f6d168b0a5ff863bbc53eae1a4d2bc6d3b522910826`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52aa5a72b36c3a0ae3e7d1771483e27a76fbe176ad7b9c5909df19accb43929`  
		Last Modified: Wed, 27 Nov 2019 00:19:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623ef70673a8d1d087393c11c4b9bdb558fd2c79600718e35536f897fd8cc62`  
		Last Modified: Wed, 27 Nov 2019 01:07:20 GMT  
		Size: 5.7 MB (5701556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802bb1630ab49e07c8c12e0217abede282fba001020ff2a88081615ac500aff`  
		Last Modified: Wed, 27 Nov 2019 01:07:17 GMT  
		Size: 13.1 KB (13103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4bebb332527fd063849b634e9771325d5f6d33382ac64692aed632000c0881`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e675cca7874d656bb6eb90fd9c5290a35a1b3bfba2b8cb2e6e92a2e0cc984e`  
		Last Modified: Wed, 27 Nov 2019 01:07:38 GMT  
		Size: 50.3 MB (50338669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931de512669a92eb87c444352698d62386d3c3f0b9e37473c757d31d38a96a`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 443.5 KB (443472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2832562b0fc65fd077e4e7af931cb4d3c075be796fc6ca0b3f2c4bf19af9b12`  
		Last Modified: Wed, 27 Nov 2019 01:08:12 GMT  
		Size: 165.0 MB (164967634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad07317e3eb0dc149bf585ca57d326d09167b3164d79d43230a431e1adc85fb7`  
		Last Modified: Wed, 27 Nov 2019 01:07:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed72b6ceb1eec3adc23bb617423c506edb26f3bea8156eae5447033b3a2d3b77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272661181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3beeee60a73ad8863ad10c6f73b5b667be0650daae1f3cdbb255cb7f7c903a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 Nov 2019 00:09:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 Nov 2019 00:12:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:12:14 GMT
ENV LANG=C.UTF-8
# Wed, 27 Nov 2019 00:12:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 Nov 2019 00:12:34 GMT
RUN rosdep init     && rosdep update
# Wed, 27 Nov 2019 00:12:38 GMT
ENV ROS_DISTRO=kinetic
# Wed, 27 Nov 2019 00:16:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 Nov 2019 00:16:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 Nov 2019 00:16:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010fc32571eae58db96ec75550ce02b64e5d668d2accf9fba61c66e29106aba`  
		Last Modified: Wed, 27 Nov 2019 00:26:20 GMT  
		Size: 6.0 MB (5959917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d247f84b81e76863e84635db36f3f0ec170dabb228e322975d435018941fb111`  
		Last Modified: Wed, 27 Nov 2019 00:26:18 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504965e33d884c9027cab5b4e3f5a0acbb234137ea604809f65454cb52f0fce4`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29294b72a432ab1b558e8df5791bfed0abea8cedfebd340ba45f5c8bd81a9542`  
		Last Modified: Wed, 27 Nov 2019 00:26:34 GMT  
		Size: 52.1 MB (52066045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c0bdce2fc2ce88f1350fc9c76be4f730229c3c1e5e83d714d75bb7a98ccb1`  
		Last Modified: Wed, 27 Nov 2019 00:26:16 GMT  
		Size: 443.6 KB (443608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d0df7ab7054f595aed83edeb45da6e20201484f80a1e7999adc630a3d3458`  
		Last Modified: Wed, 27 Nov 2019 00:27:08 GMT  
		Size: 174.2 MB (174225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cca73b15bab541593b51667aec9e966277dec7b283b47dfe2332381af7f80c`  
		Last Modified: Wed, 27 Nov 2019 00:26:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:c922dbf5109709a457c8b949dcf0ca759faa7b48d90c1ff9ff482cd6bb55d08e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:651aca230deb1169e231851d25ffb5b36688404685c374e0f323fc897738274c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.8 MB (419820444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1250f3f920f875f6b2bc8a4a326e915d83ba92071f53402bfee352396a2ebcc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm variant v7

```console
$ docker pull ros@sha256:de40681780da32d5d6f747d1920faf3e38dd7a42663047a49b13e686b14a6c70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.6 MB (372561617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc770caa4bba5169cadc2b8cb24e1e77f2e03706c572c589e91418f7a8e82903`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:211c99393be1268cacabaeba24ec112fb96088bd06524239515f33cbe3de2d46
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350489846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6625e231f3571b520ae330594c160fd4dbe67f971aadb4f1ddaf405c6cbaf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:c922dbf5109709a457c8b949dcf0ca759faa7b48d90c1ff9ff482cd6bb55d08e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:651aca230deb1169e231851d25ffb5b36688404685c374e0f323fc897738274c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.8 MB (419820444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1250f3f920f875f6b2bc8a4a326e915d83ba92071f53402bfee352396a2ebcc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:de40681780da32d5d6f747d1920faf3e38dd7a42663047a49b13e686b14a6c70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.6 MB (372561617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc770caa4bba5169cadc2b8cb24e1e77f2e03706c572c589e91418f7a8e82903`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:211c99393be1268cacabaeba24ec112fb96088bd06524239515f33cbe3de2d46
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350489846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6625e231f3571b520ae330594c160fd4dbe67f971aadb4f1ddaf405c6cbaf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:84fc7ba437aa68ce983cc72731b01cd1ef7743982e2c4772ae05264ec2554ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:05f404b4dc55651cfbc31c11c60b6720b1ccf14e8d9e162ba2cb7eb69f6075db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **773.5 MB (773488212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3df176a30d5b9f0d2d972c1ddda303a0645ae3a2b99098960dceaceae6416d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:48:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82e739253faebda68fe23e3438a5d4a85ac916cfc0de5c76f67c357af06f7c`  
		Last Modified: Thu, 31 Oct 2019 23:59:32 GMT  
		Size: 353.7 MB (353667768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:edad3a852651b2b1da0e5391ea9538441546cbf776a49475daa2fe20eaaa7fd5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.3 MB (676282419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e59aa43335e387b52f5a30cb5e55698287842324883c02e54718e618e45b6c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:48:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a81b3a0ecf65cbb43b7de242889d5bd8745a7f59bdbca437281ae1d7c25ab23`  
		Last Modified: Thu, 31 Oct 2019 23:57:17 GMT  
		Size: 303.7 MB (303720802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d89ae5809eea6a63ddded761ce7d89c4f9cfebaf747e18e79964c87de5da6995
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **686.8 MB (686786395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d859ace3a72469f58c137af988ef4bbbd6a266961e10ee2214a134f628137f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:34 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a09d61f7ac9cf80969d7a38d000373805f2f1fdaddf7b6ca82064d1c2b731d`  
		Last Modified: Thu, 31 Oct 2019 23:57:06 GMT  
		Size: 336.3 MB (336296549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:84fc7ba437aa68ce983cc72731b01cd1ef7743982e2c4772ae05264ec2554ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:05f404b4dc55651cfbc31c11c60b6720b1ccf14e8d9e162ba2cb7eb69f6075db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **773.5 MB (773488212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3df176a30d5b9f0d2d972c1ddda303a0645ae3a2b99098960dceaceae6416d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:48:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82e739253faebda68fe23e3438a5d4a85ac916cfc0de5c76f67c357af06f7c`  
		Last Modified: Thu, 31 Oct 2019 23:59:32 GMT  
		Size: 353.7 MB (353667768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:edad3a852651b2b1da0e5391ea9538441546cbf776a49475daa2fe20eaaa7fd5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.3 MB (676282419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e59aa43335e387b52f5a30cb5e55698287842324883c02e54718e618e45b6c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:48:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a81b3a0ecf65cbb43b7de242889d5bd8745a7f59bdbca437281ae1d7c25ab23`  
		Last Modified: Thu, 31 Oct 2019 23:57:17 GMT  
		Size: 303.7 MB (303720802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d89ae5809eea6a63ddded761ce7d89c4f9cfebaf747e18e79964c87de5da6995
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **686.8 MB (686786395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d859ace3a72469f58c137af988ef4bbbd6a266961e10ee2214a134f628137f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:34 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a09d61f7ac9cf80969d7a38d000373805f2f1fdaddf7b6ca82064d1c2b731d`  
		Last Modified: Thu, 31 Oct 2019 23:57:06 GMT  
		Size: 336.3 MB (336296549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:1a3564fb9102e6302c3533956a7cf46fbd2e5e99b4fff7591139a4dcab10c65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:22d0794991b136741a4ff04f31fae1314d4be900ba824c3dafbbc66f02e8c694
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **876.3 MB (876306978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a88d07e40d7489ce7fc9bceca1e5429a921cc780a700c1005a24e72e6036b28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 13:56:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:56:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 13:56:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 13:57:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 13:57:36 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 13:57:36 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 13:59:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:59:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 13:59:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 13:59:15 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 14:00:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:04:25 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2544950565d737b560035505808e64a5199cca85b079545d4fd78f1c16525`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 10.5 MB (10476343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42d47055f454d575aacdcf5cbab1322ec3be047a76940e281ad0183ebe9baf`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60170dbe616b6473d272d2399a98a75abe8736cc3b619866ccc6fb591e4cc8fc`  
		Last Modified: Sat, 23 Nov 2019 14:05:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbd35d18c3824dad4c6724f3f5d987ce438b92159b880ac3677ec0839f5e700`  
		Last Modified: Sat, 23 Nov 2019 14:05:20 GMT  
		Size: 64.8 MB (64767251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a15fb0e5240eaba2a8c00f8202135a0bd743580c6a521331e334e488483102`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 443.5 KB (443517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d23be83a08640b61250af66dca2b73b1dff9c6ef0881d87445b80ffcd71072f`  
		Last Modified: Sat, 23 Nov 2019 14:05:57 GMT  
		Size: 270.4 MB (270395770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7d953bbc957ab94aa9fda213af7ab276326175725c722f6213f2e8ed51e7b`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77530656bfd933badf8ca1a580157c9e848560c968d9f4061bce1c3e0f68d7c6`  
		Last Modified: Sat, 23 Nov 2019 14:06:23 GMT  
		Size: 108.5 MB (108473856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cead2b66bdb1e6abca2ccfd4f88c4f7cc79d2375051c6854f81aa0ed2203a`  
		Last Modified: Sat, 23 Nov 2019 14:07:54 GMT  
		Size: 376.4 MB (376367663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7c4b3ef3726bfedef9737871894067d8efa4b45f3ad92795c1fbf2bf9318f345
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **794.1 MB (794081781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8992fcff8250abeae7c26f2af780f1dd3cd961e800d0c1a5d65dc0eebff709e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:50:09 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:50:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 16:50:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 16:52:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:52:17 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 16:52:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 16:52:39 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 16:52:41 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 16:56:09 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:56:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 16:56:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 16:56:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:57:44 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 17:09:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef95a8fae2085e990d73502c6e05ccde93c612c194ca1da0c5b6473f55a015d4`  
		Last Modified: Sat, 23 Nov 2019 17:10:39 GMT  
		Size: 9.8 MB (9774200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bd6e3602ab79c0155503f16916ae260d2ae670fa254dc4b224c0eb470c26ae`  
		Last Modified: Sat, 23 Nov 2019 17:10:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93295bb4d5806786666243a0da74658a7cd7654830007d48c9686f5c21db3443`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033910be7539c98801615beb987603b1712a7d2d3e35045bc8050fe60ed12c04`  
		Last Modified: Sat, 23 Nov 2019 17:10:54 GMT  
		Size: 62.1 MB (62069083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55836e4cf09e1770edd9f21bd0791df54b45e103a3c0444002d0ae42a1b2f8d`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 443.6 KB (443559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7821c012c608a9e5a285ca0fb1008e2078aac6151cd75d57f4d8d7fe71a6e4b5`  
		Last Modified: Sat, 23 Nov 2019 17:11:45 GMT  
		Size: 224.6 MB (224573907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605780ad97ff3837df8a5213eda714dd7528192deb959fdac763e4d830062b0f`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bd548eaa022efa3a1cc404f2e23b477c82137c3bc95c4ef4bbe0b8937193a`  
		Last Modified: Sat, 23 Nov 2019 17:12:19 GMT  
		Size: 103.0 MB (102962546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8175b6945d828e200f7cb7b0c8a9d4620e446fcc88b0c5f60089119e9901d6`  
		Last Modified: Sat, 23 Nov 2019 17:14:28 GMT  
		Size: 351.1 MB (351090360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:c03a089e295adba4f4999536175a410c8f29bc8e6335afac0ca8201c95e3a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:694a593bbec7d06d369ce8ecc03d5fca1e1dbc94816f90c9ae20e04140cc169a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.6 MB (457649911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a0ba9ad0a180601405c1a0811088e4c8be7f19203358389f63ea1663bdbe82`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab7825e66a442d63e8d3687c83f3773fc0ef5080cb4e98c84379bad9a2e63e5`  
		Last Modified: Thu, 31 Oct 2019 23:58:02 GMT  
		Size: 37.8 MB (37829467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:5fbdbadff71fad92fc484d18b9f662bc4fb302bb7a5dd94b51ab6352f0cb6798
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.0 MB (405973018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d65c5d8c7025eb9971b0fcf1ebcd7c1372557887ebd8751c82cd6bf1800ce0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:44:00 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69aee5b4eb3244cf19ece2390385639a61962bf3f7dbf5e727b21f733c53908`  
		Last Modified: Thu, 31 Oct 2019 23:55:25 GMT  
		Size: 33.4 MB (33411401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b50ad31d08172dc1a9eb7ce21dbc684b7e71cee1312c1b8b6985fa35e1ab979b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386072539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a419b6b2dfc65b585a254b13c7a72325ad1eeb581e65504b5c5b41cc5bd157`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca0e2359a60340069af9f7b81962dffa64951a5629ee769ff2921495bf174bd`  
		Last Modified: Thu, 31 Oct 2019 23:55:02 GMT  
		Size: 35.6 MB (35582693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:c03a089e295adba4f4999536175a410c8f29bc8e6335afac0ca8201c95e3a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:694a593bbec7d06d369ce8ecc03d5fca1e1dbc94816f90c9ae20e04140cc169a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.6 MB (457649911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a0ba9ad0a180601405c1a0811088e4c8be7f19203358389f63ea1663bdbe82`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:42:35 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab7825e66a442d63e8d3687c83f3773fc0ef5080cb4e98c84379bad9a2e63e5`  
		Last Modified: Thu, 31 Oct 2019 23:58:02 GMT  
		Size: 37.8 MB (37829467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:5fbdbadff71fad92fc484d18b9f662bc4fb302bb7a5dd94b51ab6352f0cb6798
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.0 MB (405973018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d65c5d8c7025eb9971b0fcf1ebcd7c1372557887ebd8751c82cd6bf1800ce0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:44:00 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69aee5b4eb3244cf19ece2390385639a61962bf3f7dbf5e727b21f733c53908`  
		Last Modified: Thu, 31 Oct 2019 23:55:25 GMT  
		Size: 33.4 MB (33411401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b50ad31d08172dc1a9eb7ce21dbc684b7e71cee1312c1b8b6985fa35e1ab979b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386072539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a419b6b2dfc65b585a254b13c7a72325ad1eeb581e65504b5c5b41cc5bd157`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca0e2359a60340069af9f7b81962dffa64951a5629ee769ff2921495bf174bd`  
		Last Modified: Thu, 31 Oct 2019 23:55:02 GMT  
		Size: 35.6 MB (35582693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:378cec0f5122cac6b804a0e9677fa3c6830fe6b5c40f93e6fbdd7c8cde9bec16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:4926ee55022d2cc5ec034444ac877baae74dbdb486bc8b6c6031160a486e3ff0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.2 MB (555237633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b1cc20f8a137a7328cb00ecee1e115b30b656e40a1dcbb37d7d045db44f05e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 13:56:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:56:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 13:56:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 13:57:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 13:57:36 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 13:57:36 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 13:59:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:59:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 13:59:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 13:59:15 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 14:00:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:01:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2544950565d737b560035505808e64a5199cca85b079545d4fd78f1c16525`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 10.5 MB (10476343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42d47055f454d575aacdcf5cbab1322ec3be047a76940e281ad0183ebe9baf`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60170dbe616b6473d272d2399a98a75abe8736cc3b619866ccc6fb591e4cc8fc`  
		Last Modified: Sat, 23 Nov 2019 14:05:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbd35d18c3824dad4c6724f3f5d987ce438b92159b880ac3677ec0839f5e700`  
		Last Modified: Sat, 23 Nov 2019 14:05:20 GMT  
		Size: 64.8 MB (64767251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a15fb0e5240eaba2a8c00f8202135a0bd743580c6a521331e334e488483102`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 443.5 KB (443517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d23be83a08640b61250af66dca2b73b1dff9c6ef0881d87445b80ffcd71072f`  
		Last Modified: Sat, 23 Nov 2019 14:05:57 GMT  
		Size: 270.4 MB (270395770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7d953bbc957ab94aa9fda213af7ab276326175725c722f6213f2e8ed51e7b`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77530656bfd933badf8ca1a580157c9e848560c968d9f4061bce1c3e0f68d7c6`  
		Last Modified: Sat, 23 Nov 2019 14:06:23 GMT  
		Size: 108.5 MB (108473856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e9d30ddcecb708689fd43480ccf3a06624f4083a2ac09c02e5f7f63a227441`  
		Last Modified: Sat, 23 Nov 2019 14:06:40 GMT  
		Size: 55.3 MB (55298318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ade27f5a5b0095313259441e27e7c2d204f78f8ae0dba2b19f4ad5da166db685
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.6 MB (495574219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce65352737fe8013530ebe2b447769e3c590e9c9724aafbd1d9680f91b2c2ae9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:50:09 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:50:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 16:50:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 16:52:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:52:17 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 16:52:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 16:52:39 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 16:52:41 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 16:56:09 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:56:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 16:56:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 16:56:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:57:44 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:59:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef95a8fae2085e990d73502c6e05ccde93c612c194ca1da0c5b6473f55a015d4`  
		Last Modified: Sat, 23 Nov 2019 17:10:39 GMT  
		Size: 9.8 MB (9774200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bd6e3602ab79c0155503f16916ae260d2ae670fa254dc4b224c0eb470c26ae`  
		Last Modified: Sat, 23 Nov 2019 17:10:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93295bb4d5806786666243a0da74658a7cd7654830007d48c9686f5c21db3443`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033910be7539c98801615beb987603b1712a7d2d3e35045bc8050fe60ed12c04`  
		Last Modified: Sat, 23 Nov 2019 17:10:54 GMT  
		Size: 62.1 MB (62069083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55836e4cf09e1770edd9f21bd0791df54b45e103a3c0444002d0ae42a1b2f8d`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 443.6 KB (443559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7821c012c608a9e5a285ca0fb1008e2078aac6151cd75d57f4d8d7fe71a6e4b5`  
		Last Modified: Sat, 23 Nov 2019 17:11:45 GMT  
		Size: 224.6 MB (224573907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605780ad97ff3837df8a5213eda714dd7528192deb959fdac763e4d830062b0f`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bd548eaa022efa3a1cc404f2e23b477c82137c3bc95c4ef4bbe0b8937193a`  
		Last Modified: Sat, 23 Nov 2019 17:12:19 GMT  
		Size: 103.0 MB (102962546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252d7b4486139a1b1b98cda0bb2748afcedbb486339765c728c3a67936281540`  
		Last Modified: Sat, 23 Nov 2019 17:12:40 GMT  
		Size: 52.6 MB (52582798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:c922dbf5109709a457c8b949dcf0ca759faa7b48d90c1ff9ff482cd6bb55d08e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:651aca230deb1169e231851d25ffb5b36688404685c374e0f323fc897738274c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.8 MB (419820444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1250f3f920f875f6b2bc8a4a326e915d83ba92071f53402bfee352396a2ebcc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:de40681780da32d5d6f747d1920faf3e38dd7a42663047a49b13e686b14a6c70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.6 MB (372561617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc770caa4bba5169cadc2b8cb24e1e77f2e03706c572c589e91418f7a8e82903`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:211c99393be1268cacabaeba24ec112fb96088bd06524239515f33cbe3de2d46
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350489846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6625e231f3571b520ae330594c160fd4dbe67f971aadb4f1ddaf405c6cbaf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:c922dbf5109709a457c8b949dcf0ca759faa7b48d90c1ff9ff482cd6bb55d08e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:651aca230deb1169e231851d25ffb5b36688404685c374e0f323fc897738274c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.8 MB (419820444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1250f3f920f875f6b2bc8a4a326e915d83ba92071f53402bfee352396a2ebcc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:41:39 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5942e3fe617dcb8b6fb59a1e4dad8ba632de0a6bc9f5558f310178e6a0ad7`  
		Last Modified: Thu, 31 Oct 2019 23:57:47 GMT  
		Size: 68.3 MB (68331487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:de40681780da32d5d6f747d1920faf3e38dd7a42663047a49b13e686b14a6c70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.6 MB (372561617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc770caa4bba5169cadc2b8cb24e1e77f2e03706c572c589e91418f7a8e82903`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:43:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cba56633327b2b6290cafdfd428c01aee949bb8ada7b71aa2ecd83f6a60c9b`  
		Last Modified: Thu, 31 Oct 2019 23:55:04 GMT  
		Size: 60.2 MB (60249848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:211c99393be1268cacabaeba24ec112fb96088bd06524239515f33cbe3de2d46
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350489846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6625e231f3571b520ae330594c160fd4dbe67f971aadb4f1ddaf405c6cbaf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
# Thu, 31 Oct 2019 23:34:46 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca70e2ac1a897857766a33b3e58dfaeb6bf68fe80fc54284cb85ee98feacec2`  
		Last Modified: Thu, 31 Oct 2019 23:54:41 GMT  
		Size: 62.8 MB (62839599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:2817997fac4a80aa6555f9df18fb6b34efb07d5f94a2f2ae21482f5b5fa8f5d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:5e25cc6d0f46e04456f5f2c96f3ee4855242b745e46acf8405977832189676ad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.9 MB (499939315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc4d996b61a00cbf8e1104ca7d408e4d0cda60887fe77b0b47f3acde2ba11aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 13:56:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:56:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 13:56:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 13:57:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 13:57:36 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 13:57:36 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 13:59:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:59:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 13:59:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 13:59:15 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 14:00:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2544950565d737b560035505808e64a5199cca85b079545d4fd78f1c16525`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 10.5 MB (10476343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42d47055f454d575aacdcf5cbab1322ec3be047a76940e281ad0183ebe9baf`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60170dbe616b6473d272d2399a98a75abe8736cc3b619866ccc6fb591e4cc8fc`  
		Last Modified: Sat, 23 Nov 2019 14:05:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbd35d18c3824dad4c6724f3f5d987ce438b92159b880ac3677ec0839f5e700`  
		Last Modified: Sat, 23 Nov 2019 14:05:20 GMT  
		Size: 64.8 MB (64767251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a15fb0e5240eaba2a8c00f8202135a0bd743580c6a521331e334e488483102`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 443.5 KB (443517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d23be83a08640b61250af66dca2b73b1dff9c6ef0881d87445b80ffcd71072f`  
		Last Modified: Sat, 23 Nov 2019 14:05:57 GMT  
		Size: 270.4 MB (270395770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7d953bbc957ab94aa9fda213af7ab276326175725c722f6213f2e8ed51e7b`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77530656bfd933badf8ca1a580157c9e848560c968d9f4061bce1c3e0f68d7c6`  
		Last Modified: Sat, 23 Nov 2019 14:06:23 GMT  
		Size: 108.5 MB (108473856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c56b9690c6dab8a4dbce7c943678ef6d6b4ecff03937d0f61bb05e5b243f148f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.0 MB (442991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1437b75ecd64c0081c70964b4c7e5a8cd7ebf346316751a59e7b76a3d99d9576`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:50:09 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:50:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 16:50:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 16:52:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:52:17 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 16:52:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 16:52:39 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 16:52:41 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 16:56:09 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:56:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 16:56:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 16:56:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:57:44 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef95a8fae2085e990d73502c6e05ccde93c612c194ca1da0c5b6473f55a015d4`  
		Last Modified: Sat, 23 Nov 2019 17:10:39 GMT  
		Size: 9.8 MB (9774200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bd6e3602ab79c0155503f16916ae260d2ae670fa254dc4b224c0eb470c26ae`  
		Last Modified: Sat, 23 Nov 2019 17:10:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93295bb4d5806786666243a0da74658a7cd7654830007d48c9686f5c21db3443`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033910be7539c98801615beb987603b1712a7d2d3e35045bc8050fe60ed12c04`  
		Last Modified: Sat, 23 Nov 2019 17:10:54 GMT  
		Size: 62.1 MB (62069083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55836e4cf09e1770edd9f21bd0791df54b45e103a3c0444002d0ae42a1b2f8d`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 443.6 KB (443559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7821c012c608a9e5a285ca0fb1008e2078aac6151cd75d57f4d8d7fe71a6e4b5`  
		Last Modified: Sat, 23 Nov 2019 17:11:45 GMT  
		Size: 224.6 MB (224573907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605780ad97ff3837df8a5213eda714dd7528192deb959fdac763e4d830062b0f`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bd548eaa022efa3a1cc404f2e23b477c82137c3bc95c4ef4bbe0b8937193a`  
		Last Modified: Sat, 23 Nov 2019 17:12:19 GMT  
		Size: 103.0 MB (102962546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:c225ae02fcd30f30ce73c47815d90c087b506f140e04a608e82ed687569260da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:aad07e5d5309164c1784407cb0cd07481e4ac2daa0384139573c58a2a2e38e66
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351488957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233543612bae6e6efffb9be878d55c58465a7720bd3be11a46739c9a6aa04be2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:0aec1d3386a9e3e7638bca5130785d69b19b08f2441325fb8d84598beea88f38
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.3 MB (312311769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2414ed77684725dede5e3c22b4a04cf402f41a132b04d82390a7fbb791fc46`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:93d19d913470718702f9ee4483765df2ce4d292b0adef2b705e4931bba56c8a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287650247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c5c0af66851e73a43e3280fcb89e7c76fabac6d56b84d4eb3cdb765be28455`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:c225ae02fcd30f30ce73c47815d90c087b506f140e04a608e82ed687569260da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:aad07e5d5309164c1784407cb0cd07481e4ac2daa0384139573c58a2a2e38e66
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351488957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233543612bae6e6efffb9be878d55c58465a7720bd3be11a46739c9a6aa04be2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:20:35 GMT
ADD file:a48a5dc1b9dbfc632f6cf86fe27b770b63f07a115c98c4465dc184e303a4efa1 in / 
# Thu, 31 Oct 2019 22:20:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:20:37 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:35:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:42 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:35:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:36:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:36:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:37:00 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:37:00 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:40:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:40:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:40:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:40:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7ddbc47eeb70dc7f08e410a6667948b87ff3883024eb41478b44ef9a81bf400c`  
		Last Modified: Wed, 30 Oct 2019 00:25:34 GMT  
		Size: 26.7 MB (26688847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bbdc448b7263673926b8fe2e88491e5083a8b4b06ddfabf311f2fc5f27e2ff`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 35.4 KB (35362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b70e3904492c753652606df4726430426f42ea56e06ea924d6fea7ae162a1`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d437916d5781043432f2d72608049dcf74ddbd27daa01a25fa63c8f1b9adc4`  
		Last Modified: Thu, 31 Oct 2019 22:21:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9b01e3e432647233f9f035261d029b8747860c89497091395a3385eb8ed7ff`  
		Last Modified: Thu, 31 Oct 2019 23:56:28 GMT  
		Size: 837.3 KB (837344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb7e096fb19a76ff587feaff77fd96d62aa1a9827cd2da7c7dbccae43ce293`  
		Last Modified: Thu, 31 Oct 2019 23:56:29 GMT  
		Size: 6.8 MB (6776244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516bdffd8ca21a3c0ff804eaf5721cd22a1adc90b21df568c1f20cd56f5c9c8e`  
		Last Modified: Thu, 31 Oct 2019 23:56:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60339fb0d35d575b6ed15f38b9b98d3da747d2df9e7c49b1dfdfbf96bc51a49a`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a7a7d6ca1c302f8bc37ca9a3680d4b900bf850eaa2971bab6d5d74ebbf16`  
		Last Modified: Thu, 31 Oct 2019 23:56:42 GMT  
		Size: 55.1 MB (55059632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa796f177cf039457e16cdefa80513cc6a774e1d856c7dee0e1b43a7afda0b`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 432.8 KB (432773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960f5a11411c332a54546cb616050312a57fdd8010c5a6df55fc6441dc4b48a`  
		Last Modified: Thu, 31 Oct 2019 23:57:24 GMT  
		Size: 261.7 MB (261655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f77b2b02e40a07d89e3ce1d91b1f5865c9004e65b40696cca2c75dabd04cb9`  
		Last Modified: Thu, 31 Oct 2019 23:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:0aec1d3386a9e3e7638bca5130785d69b19b08f2441325fb8d84598beea88f38
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.3 MB (312311769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2414ed77684725dede5e3c22b4a04cf402f41a132b04d82390a7fbb791fc46`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 23:05:17 GMT
ADD file:f26a9806a1c17950a5032204bfe5c5b34e4eb2396e512d30edeaf23577fa5a06 in / 
# Thu, 31 Oct 2019 23:05:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 23:05:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 23:05:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 23:05:24 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:36:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:06 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:37:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:37:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:38:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:38:21 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:38:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:38:40 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:38:40 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:41:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:41:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:41:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:41:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:60341935f70d34eb6a96ec71514be0b8c977900067664076335f115cfbb73687`  
		Last Modified: Thu, 31 Oct 2019 23:07:22 GMT  
		Size: 22.3 MB (22274856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2b7c380f80ba0f87075cb19d83f61c3b38482aa1dc0893e0e7185471348ac`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 35.5 KB (35460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9d3d2adfb541c899c161be416e7ad735dcb5c8516061ace68a953a5d9f57f7`  
		Last Modified: Thu, 31 Oct 2019 23:07:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac0b57271f848c7c02d0795a4f579610e3956c1646254e7809dcdb06c540dbc`  
		Last Modified: Thu, 31 Oct 2019 23:07:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c76bf825964552e921714352bc0fa3cf3e1a9bfac1931e7a34c965aa086af40`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 837.9 KB (837935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b0dd98d6ed1afe3a0025e14f9620fa734566e7e27e9a8e7265ede0f9da0847`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 5.6 MB (5627036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365caca88c25382d5e1922b657a282a7f41c049b8a30a53bc5bc153f0898349`  
		Last Modified: Thu, 31 Oct 2019 23:53:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e4ba19845124367cdf251aa36ff0a3539ca395b561a58952ddaa3956dbe16`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee48456c2367ed4832bc64306a0c10efce837c82109cc224066be5870f0402`  
		Last Modified: Thu, 31 Oct 2019 23:53:42 GMT  
		Size: 50.1 MB (50099454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef38b03fa65c6f3a5a9eb09ba1703a9885ff223f1c390ef19f6ae77f2d0683`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 432.8 KB (432785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ebac3b94788402ec3ed25e41f7ffdad5074ba15bc4b8a3aa36bf7cee6337c`  
		Last Modified: Thu, 31 Oct 2019 23:54:35 GMT  
		Size: 233.0 MB (233001370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b240f898b7616de2b0b7b23b4027f0d7d85f2dcd2563ebb70d88d1a5dee9cc`  
		Last Modified: Thu, 31 Oct 2019 23:53:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:93d19d913470718702f9ee4483765df2ce4d292b0adef2b705e4931bba56c8a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287650247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c5c0af66851e73a43e3280fcb89e7c76fabac6d56b84d4eb3cdb765be28455`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:28:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:36 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:28:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 31 Oct 2019 23:28:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 31 Oct 2019 23:29:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LANG=C.UTF-8
# Thu, 31 Oct 2019 23:29:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 31 Oct 2019 23:30:09 GMT
RUN rosdep init     && rosdep update
# Thu, 31 Oct 2019 23:30:09 GMT
ENV ROS_DISTRO=melodic
# Thu, 31 Oct 2019 23:33:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:33:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 31 Oct 2019 23:33:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 31 Oct 2019 23:33:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26a9f66c6d06a0b61908fc5ae522ef1d40f49507b344c85bfeca37e056ddf8`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 837.8 KB (837784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46637339d4876ccd94fa6cf185787053d210ea7671bd037b1cc685f639694b99`  
		Last Modified: Thu, 31 Oct 2019 23:53:12 GMT  
		Size: 6.1 MB (6093384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b0986006f87a1dd1179f2a70f0c2e45cc4e05cd20efec9df579260c32eea9`  
		Last Modified: Thu, 31 Oct 2019 23:53:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690f53d678ab501a0f5ccceced3d957bab3f1a38ced8cb247bca3be89039247`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da28666899a4aa50257b37de5918c7f07f7db6fa81d5d2f14a5eb3755c435d`  
		Last Modified: Thu, 31 Oct 2019 23:53:26 GMT  
		Size: 52.8 MB (52831522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c0f9558971467bab1b8a1c2154458de0466a667501c6dcb2261bcec837491`  
		Last Modified: Thu, 31 Oct 2019 23:53:10 GMT  
		Size: 432.8 KB (432811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38309afe4efb92d963c50db1db71d365c928407d68c681b44f730ccfd1c95e99`  
		Last Modified: Thu, 31 Oct 2019 23:54:13 GMT  
		Size: 203.7 MB (203698274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf59a4edb742add8b245acdb6ffaefb00a747d9e6812651a2601e7efc47c0fe`  
		Last Modified: Thu, 31 Oct 2019 23:53:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:017c481136d5d1ae16c5c48e1ef47e109a1719a77784d78e6369b480ffd1dbfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:2ea2a0a209e14040e562bd968747d86b302bb14acbf768ee543aa3b43c7c826f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.5 MB (391465459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16d26a9cefc0328b237c453bdd58537fdb3ab75dcb2682751e8f6612d3116d2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 13:56:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:56:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 13:56:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 13:57:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 13:57:26 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 13:57:36 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 13:57:36 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 13:59:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 13:59:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 13:59:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 13:59:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2544950565d737b560035505808e64a5199cca85b079545d4fd78f1c16525`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 10.5 MB (10476343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42d47055f454d575aacdcf5cbab1322ec3be047a76940e281ad0183ebe9baf`  
		Last Modified: Sat, 23 Nov 2019 14:05:08 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60170dbe616b6473d272d2399a98a75abe8736cc3b619866ccc6fb591e4cc8fc`  
		Last Modified: Sat, 23 Nov 2019 14:05:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbd35d18c3824dad4c6724f3f5d987ce438b92159b880ac3677ec0839f5e700`  
		Last Modified: Sat, 23 Nov 2019 14:05:20 GMT  
		Size: 64.8 MB (64767251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a15fb0e5240eaba2a8c00f8202135a0bd743580c6a521331e334e488483102`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 443.5 KB (443517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d23be83a08640b61250af66dca2b73b1dff9c6ef0881d87445b80ffcd71072f`  
		Last Modified: Sat, 23 Nov 2019 14:05:57 GMT  
		Size: 270.4 MB (270395770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7d953bbc957ab94aa9fda213af7ab276326175725c722f6213f2e8ed51e7b`  
		Last Modified: Sat, 23 Nov 2019 14:05:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:600669b540eeb1afb4e4410623767f463ec92be5b4171ade07835cb77b0ae0f0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.0 MB (340028875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bebe745e00f3f5e123626f5d3db80720aada3eb09ef307bda14d57e63ac93c1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 16:50:09 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:50:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Nov 2019 16:50:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Nov 2019 16:52:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:52:17 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 16:52:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Nov 2019 16:52:39 GMT
RUN rosdep init     && rosdep update
# Sat, 23 Nov 2019 16:52:41 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Nov 2019 16:56:09 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:56:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Nov 2019 16:56:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Nov 2019 16:56:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef95a8fae2085e990d73502c6e05ccde93c612c194ca1da0c5b6473f55a015d4`  
		Last Modified: Sat, 23 Nov 2019 17:10:39 GMT  
		Size: 9.8 MB (9774200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bd6e3602ab79c0155503f16916ae260d2ae670fa254dc4b224c0eb470c26ae`  
		Last Modified: Sat, 23 Nov 2019 17:10:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93295bb4d5806786666243a0da74658a7cd7654830007d48c9686f5c21db3443`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033910be7539c98801615beb987603b1712a7d2d3e35045bc8050fe60ed12c04`  
		Last Modified: Sat, 23 Nov 2019 17:10:54 GMT  
		Size: 62.1 MB (62069083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55836e4cf09e1770edd9f21bd0791df54b45e103a3c0444002d0ae42a1b2f8d`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 443.6 KB (443559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7821c012c608a9e5a285ca0fb1008e2078aac6151cd75d57f4d8d7fe71a6e4b5`  
		Last Modified: Sat, 23 Nov 2019 17:11:45 GMT  
		Size: 224.6 MB (224573907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605780ad97ff3837df8a5213eda714dd7528192deb959fdac763e4d830062b0f`  
		Last Modified: Sat, 23 Nov 2019 17:10:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
