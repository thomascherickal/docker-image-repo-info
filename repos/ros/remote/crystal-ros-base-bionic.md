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
