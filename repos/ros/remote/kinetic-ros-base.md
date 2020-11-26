## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:7276c5926b7179e20c3d0a6f0ef96950a7226b3f417ed7902d0f9cedf792f440
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c6eddc6699cf6cc461bb5bb4a76a98427f4f5358d6c4849b9caf5b6756dbfa28
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.4 MB (359421311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e624fbb5b82720762236399de0d7dd54b7170991648197d0f19cceb1fe990da3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:31:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:31:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 19:31:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 23 Oct 2020 19:31:13 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 19:31:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 19:31:14 GMT
ENV ROS_DISTRO=kinetic
# Fri, 23 Oct 2020 19:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:33:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 23 Oct 2020 19:33:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 19:33:16 GMT
CMD ["bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Oct 2020 19:34:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6506cb466c9caaf79d9099a213fd08adcba6f018cd8360f20c05919d8a12fae1`  
		Last Modified: Fri, 23 Oct 2020 19:54:17 GMT  
		Size: 5.4 MB (5362322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb38ec3e7afd32045ced91202a93a356861f16a3e976adfdd92f79b3a5675c`  
		Last Modified: Fri, 23 Oct 2020 19:54:14 GMT  
		Size: 14.7 KB (14746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b35dcd31ec1c224bcbae1f0b564049e4cc416771f17352a0ce2a19c1c2feb`  
		Last Modified: Fri, 23 Oct 2020 19:54:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210b782ec4e83a272258b58e4cc1dca9d9da861b0f15f0bf000821cb56972000`  
		Last Modified: Fri, 23 Oct 2020 19:55:01 GMT  
		Size: 187.1 MB (187132234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff55477f12b851aca47ff841b7b4b4d03002c8e5a4eefdc02a54f0bc97dc682c`  
		Last Modified: Fri, 23 Oct 2020 19:54:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b978f6826469aa735fd206950cac076d40ad772a7019454ae579ef37ba2804c`  
		Last Modified: Fri, 23 Oct 2020 19:55:19 GMT  
		Size: 57.2 MB (57240615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95484c10cdcfce2447d30afa3263ea2cfb1e8228eb5ef30751980c9485634ad9`  
		Last Modified: Fri, 23 Oct 2020 19:55:07 GMT  
		Size: 266.9 KB (266861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2217cfe9462ea83e9ef9a84ddd8434a431697950a1d53bc8048ed83a95375db`  
		Last Modified: Fri, 23 Oct 2020 19:55:22 GMT  
		Size: 63.6 MB (63576856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:2a300b8894366660db995a5b167607fdec548522a3b16d1c76a6aafb068c4f04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.3 MB (311252751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f312c3959c85b993decbfe4c5565d0442e4af0819f28714f4978f8a4ec8e2a55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 25 Nov 2020 23:01:00 GMT
ADD file:0947a09b11d2a3286469b4ddf6d3d58881839b8c4377d343e475d0e66eef9b7d in / 
# Wed, 25 Nov 2020 23:01:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 23:01:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:01:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 23:01:12 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:01:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:01:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 26 Nov 2020 00:01:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 26 Nov 2020 00:01:56 GMT
ENV LANG=C.UTF-8
# Thu, 26 Nov 2020 00:01:59 GMT
ENV LC_ALL=C.UTF-8
# Thu, 26 Nov 2020 00:02:00 GMT
ENV ROS_DISTRO=kinetic
# Thu, 26 Nov 2020 00:04:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:04:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 26 Nov 2020 00:04:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 26 Nov 2020 00:04:51 GMT
CMD ["bash"]
# Thu, 26 Nov 2020 00:05:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:05:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 26 Nov 2020 00:07:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bc86a2fe0a9b47f715e84e5bd1286da57dd7a79808c3da3571e7545fbb90af7`  
		Last Modified: Mon, 02 Nov 2020 23:20:03 GMT  
		Size: 39.9 MB (39902208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adf0a70ddb4a67405dcca7eecf8c4f56d13faa0de2f12a5cdfc5ee63d72a681`  
		Last Modified: Wed, 25 Nov 2020 23:02:40 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5475b6908bf78ed05b18766116eaeb7fbce1ffeee65c72b2f7bfdf420097cf6`  
		Last Modified: Wed, 25 Nov 2020 23:02:39 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed78ff2520e3b2a6193c0dccf58ab7b2adcb9bd51165f163021650e823ab0a3`  
		Last Modified: Wed, 25 Nov 2020 23:02:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8d7167c262fee184b690ddaaaa36f74accf49367d841ec614677e386671cab`  
		Last Modified: Thu, 26 Nov 2020 01:06:33 GMT  
		Size: 4.6 MB (4615075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ae19f7a2781c0f4501007baa969545ec9a431cd9a42edb067ceb5609cf8fed`  
		Last Modified: Thu, 26 Nov 2020 01:06:31 GMT  
		Size: 14.7 KB (14747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad72b5255dcd2bd45b8fb55efb9527cfc69329e8e7467c9c1d9e000d7706801`  
		Last Modified: Thu, 26 Nov 2020 01:06:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81d94c0bb6a7b5c6ee98ed32b19d7e66ac343a326e28029377ac8cd6c2954b6`  
		Last Modified: Thu, 26 Nov 2020 01:07:31 GMT  
		Size: 168.1 MB (168052966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2ba32400064d1c993d9cb1298e0b1ab4336f1dc86962ab4563f48de01ec7f`  
		Last Modified: Thu, 26 Nov 2020 01:06:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa280c4eb10e8d699199b4336dad187219d59c5f7ef44455a7faba6aee862949`  
		Last Modified: Thu, 26 Nov 2020 01:08:00 GMT  
		Size: 42.9 MB (42892583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc052190a86d8804cae67f64c16f18130556e5efc6565c96a1377c7121b563f3`  
		Last Modified: Thu, 26 Nov 2020 01:07:40 GMT  
		Size: 269.0 KB (268958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd96cd1f3a28fff7b34af7b9b69724991babc1fbb28431b168f6f9c6046067a`  
		Last Modified: Thu, 26 Nov 2020 01:07:58 GMT  
		Size: 55.5 MB (55504255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3ae9c723ed34764d4814263e2f4c31ae18f37ec16fb029db68d32a54239587a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325210230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68a1fbb059fd2e02b85ccde6bf07acdd8ec4d6df1c1c1eb488014de0d557a29`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:49:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:49:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 25 Nov 2020 23:49:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 25 Nov 2020 23:49:35 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 23:49:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 25 Nov 2020 23:49:37 GMT
ENV ROS_DISTRO=kinetic
# Wed, 25 Nov 2020 23:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:52:43 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 25 Nov 2020 23:52:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 25 Nov 2020 23:52:45 GMT
CMD ["bash"]
# Wed, 25 Nov 2020 23:53:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:53:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 25 Nov 2020 23:54:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd8c88b81ce1d2014f2eb69aaab1bc6a43960f2bb541599f95364f321154dc`  
		Last Modified: Thu, 26 Nov 2020 01:03:54 GMT  
		Size: 4.8 MB (4820331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8577196a9ddabebca148188e299af2498816d078cb0216b79df969f5667f260`  
		Last Modified: Thu, 26 Nov 2020 01:03:53 GMT  
		Size: 14.7 KB (14746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ba2ccc0d2f632b253e7332accd9d84f2ed32f50a82134983f585bf9e7dbc05`  
		Last Modified: Thu, 26 Nov 2020 01:03:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3a269cf6a9c0ba408a1f77dac4e7568b1f7017c6ed6a0ad2ae23f74801a6c6`  
		Last Modified: Thu, 26 Nov 2020 01:04:45 GMT  
		Size: 176.0 MB (176025998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca44a362de8e65b18999bc0b7b13fa0fe54b2c5b6cb4e9c042f555a46fb50b18`  
		Last Modified: Thu, 26 Nov 2020 01:03:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6ed45fc6b0d4222cae599c87c4993ee9e8a2e9423239ad253ad23a7e45f89f`  
		Last Modified: Thu, 26 Nov 2020 01:05:07 GMT  
		Size: 46.0 MB (45953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a8b665df2168cbe4bc65dbb617c06b38dc04bfd2fa668933eb0c8455e6a261`  
		Last Modified: Thu, 26 Nov 2020 01:04:55 GMT  
		Size: 268.9 KB (268918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c5ef18da559def44f4cb7b0151a5a1d95888450beaaabe8a15a9331cf6e9db`  
		Last Modified: Thu, 26 Nov 2020 01:05:10 GMT  
		Size: 57.3 MB (57298744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
