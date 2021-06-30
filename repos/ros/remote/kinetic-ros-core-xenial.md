## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:2fe2471dbc1bdc716bcff500fcdc275fd440ef4918c71c5cf64c4db5bb4fa958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:518144280d667d4d39a1faeb6f12c17660a8512481d465284abf35d0534ddfe3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (239048959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d66e4fac4966a3a5ea42ff8380d8612f9f695bb40df1175b9cab63934abadc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:07:24 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 22:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 22:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 22:07:29 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:11:07 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:11:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:11:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee46e5af810171e31b4b35e27558f45782fb006de122f2546e5ac6223e0a55`  
		Last Modified: Fri, 18 Jun 2021 02:21:24 GMT  
		Size: 5.4 MB (5364295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1bbf7dea9f8451ba82aa6d7a0dd94e19f79a820bab77c9980722df7187cd8`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662b1269a41e6de032798855bcf879ce4770adf199f4fb6262baf94540812a1`  
		Last Modified: Tue, 29 Jun 2021 22:21:47 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f759c9d3424a8c63bb35d5cf994f8fe5fdcacc4a63563c57df046411fe2df12d`  
		Last Modified: Tue, 29 Jun 2021 22:22:33 GMT  
		Size: 187.2 MB (187170601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe81202a2c2cdc4ef1924d3686a52ba451b7e6afaf7cabb4b59a45fe2670e5`  
		Last Modified: Tue, 29 Jun 2021 22:21:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:2bf27c4d7af247414dfa948feb54131c5ca8f906d7968ffcea1a22aed61b78c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212985157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afffe9a36c5ca012f47b06ade09be86fbec56c9228e931f9bc8ac792276ef2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:33:04 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Thu, 17 Jun 2021 23:33:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:33:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:33:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:33:07 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 02:34:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:34:11 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 30 Jun 2021 02:34:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:34:15 GMT
ENV ROS_DISTRO=kinetic
# Wed, 30 Jun 2021 02:36:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:36:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:36:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:36:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e7436b523284825c35db6cb48a7c20c8d5388815695277126f528b2b4537`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c9e5711d0203aa41ec7750be25bd3bdd00b90388fde5a0d603523354eff4e`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1eba314dc97cbd3e70e1b857a42881405eefe61a235d56722dbf0df809d73`  
		Last Modified: Thu, 17 Jun 2021 23:36:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039754e3bda187ac885dbc6ea3dc6bbfd4a1aed5afce46ecf40ca07fbe87b0f`  
		Last Modified: Wed, 30 Jun 2021 03:05:35 GMT  
		Size: 4.6 MB (4615773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ff638d0d10c8b0d911bf78282eaf605fc10003c9fc21d7b69ff3955685fd5`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c28c2c2718facbfc1ea2b26b1171d27e91e51131a2f3f64dccc84611cd6b2f`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0cc68213e763d6c5f8cb3b90944257ec441165b2395349fc19d6296bfb08`  
		Last Modified: Wed, 30 Jun 2021 03:07:24 GMT  
		Size: 168.0 MB (168039692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52efdad1bfd831982a7951811b0e06f99add6c5afd2cfaca9c32ec25209c2c3`  
		Last Modified: Wed, 30 Jun 2021 03:05:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bdb0d5f7a8cc3f25d7520cd12ffb30f67e7ce4adfd35dde79b134fbeeb5f2da4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.1 MB (222100105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59af12ff68b67fedfd529212d437fa5431f5eda15825ee64aeeacdf42ba1e75a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:08:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 21:59:47 GMT
RUN echo "deb http://snapshots.ros.org/kinetic/final/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 29 Jun 2021 21:59:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LANG=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Jun 2021 21:59:50 GMT
ENV ROS_DISTRO=kinetic
# Tue, 29 Jun 2021 22:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 22:00:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Jun 2021 22:00:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Jun 2021 22:00:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c5516d91222e4ab20e59131499e0e6634037398137ff5e8fafe63f23745db`  
		Last Modified: Fri, 18 Jun 2021 01:30:44 GMT  
		Size: 4.8 MB (4821026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30d6562a575773abc9b108ad53c629e8496d186807df65e6660efb22d5f7a4`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45e27cc7ec4d3b07844cc3f12669669c39101cdf3fee4eb84bf481d0b17dfa`  
		Last Modified: Tue, 29 Jun 2021 22:07:13 GMT  
		Size: 15.3 KB (15300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63efc4a6cf0fe338b0f5350e293cc4804d22786c6ba065861d49013ca496177`  
		Last Modified: Tue, 29 Jun 2021 22:07:45 GMT  
		Size: 176.0 MB (176021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2607d8fbe58766d2c28020314ab65451f61b792635c9aa739a71bc95677e6c`  
		Last Modified: Tue, 29 Jun 2021 22:07:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
