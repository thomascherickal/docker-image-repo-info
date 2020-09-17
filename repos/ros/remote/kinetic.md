## `ros:kinetic`

```console
$ docker pull ros@sha256:437c2c306665b130fbc4379f26c47037abdcf25d137a5b288ba1165daf86a5ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:8bdcc587802f7e849cbab96753d1f4a3247fb3bc751707c94bc8371c9ab8003c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.1 MB (358090967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:572bdbeae88818fae47e988b1fc25dfa5007e1531a28c127f0629f6faa674ae0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:15:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:15:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 01:15:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Sep 2020 01:15:55 GMT
ENV LANG=C.UTF-8
# Thu, 17 Sep 2020 01:15:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Sep 2020 01:15:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 17 Sep 2020 01:18:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:18:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 17 Sep 2020 01:18:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 01:18:16 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 01:18:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:19:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 01:19:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9762a0cc4800a3b0af620830f7d545e97cae71d94f377d41d6f874e9535f7e12`  
		Last Modified: Thu, 17 Sep 2020 02:02:21 GMT  
		Size: 5.4 MB (5362198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3691926ea673c1d5eb1bf0e552338b220f86fbff80cc8787a58d98a92565e685`  
		Last Modified: Thu, 17 Sep 2020 02:02:20 GMT  
		Size: 14.7 KB (14746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962699b73ed9d0689efa306fe98b9f6ac76db76c42d536a0ed6abbe335709853`  
		Last Modified: Thu, 17 Sep 2020 02:02:20 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782a00058e494bf5ee7df8c7225645c54f64f8c2e35f6e3d4b4f01765e792ce`  
		Last Modified: Thu, 17 Sep 2020 02:03:09 GMT  
		Size: 187.1 MB (187139790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d02d91599f16518ae25311a5807de849fb76bd8b3e2e8d35effff58f07a4a02`  
		Last Modified: Thu, 17 Sep 2020 02:02:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02c98ff917faf49f028fc3f96fa1e7d3442aed429a939305d207e24c12970a0`  
		Last Modified: Thu, 17 Sep 2020 02:03:27 GMT  
		Size: 57.2 MB (57240346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da27afe15fa59f3c31ad8a4afcbda578bc720f639c95fdbd32610d59af8346eb`  
		Last Modified: Thu, 17 Sep 2020 02:03:14 GMT  
		Size: 264.6 KB (264620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07639d4e0724e658775a73e248e1d48221efe5778eb38b6b2c06e3b7ff5ad77`  
		Last Modified: Thu, 17 Sep 2020 02:03:30 GMT  
		Size: 63.6 MB (63576493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:8372c414cbbbae21cf90832b620a31e484f1e92645fd75f334e7df9d27ec8693
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310384514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaf9c1dfbfa400de860ddeb7add2531ee94ae40de70818818bdcf610f5044bd3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:30:05 GMT
ADD file:38aaa478c79aa248bad103715a39948793d797d37812d22469c22ee5d851ae7d in / 
# Wed, 16 Sep 2020 22:30:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:30:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:30:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:30:14 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:30:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:30:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Sep 2020 23:30:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Sep 2020 23:30:59 GMT
ENV LANG=C.UTF-8
# Wed, 16 Sep 2020 23:31:00 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Sep 2020 23:31:01 GMT
ENV ROS_DISTRO=kinetic
# Wed, 16 Sep 2020 23:33:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:33:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 16 Sep 2020 23:33:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Sep 2020 23:33:30 GMT
CMD ["bash"]
# Wed, 16 Sep 2020 23:34:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:34:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 16 Sep 2020 23:35:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13ff11dca1d6052e4025732a8fa027aecbd6e55b19a6b9ad7b324d0ad5b188be`  
		Last Modified: Mon, 07 Sep 2020 15:58:48 GMT  
		Size: 39.1 MB (39075749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724bf755e43234a743c552c2b8d8b994728e9584ef07a48b3409fbd838d112f2`  
		Last Modified: Wed, 16 Sep 2020 22:31:23 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bc444073b632a9a70a0c9afdeb3b85fd5825c467bd64b3e3e345634a1633be`  
		Last Modified: Wed, 16 Sep 2020 22:31:23 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c632cb71c9b8f4e9c5e410f5d672570841e16446869dc106b325d823a27b0`  
		Last Modified: Wed, 16 Sep 2020 22:31:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0835beff39d122e815f0433befb142297ab6b7771f0990fa96cca767a2c16ace`  
		Last Modified: Thu, 17 Sep 2020 00:16:45 GMT  
		Size: 4.6 MB (4614907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa64db46faff33588a4ccb736d40ea57cad734b1e496c3616387f474f25c8edf`  
		Last Modified: Thu, 17 Sep 2020 00:16:44 GMT  
		Size: 14.7 KB (14746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca6575d77d7493b73890260a28c5bf3d7754bac66f6ae4d73ece4335daceb0`  
		Last Modified: Thu, 17 Sep 2020 00:16:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc46ca1f532310386ae171b12231e87c45988bfeca6cf46cf0ed7d9f6757aeb`  
		Last Modified: Thu, 17 Sep 2020 00:18:04 GMT  
		Size: 168.0 MB (168018198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb77439a4d5d964695007d0030c7e8fbce96a663c5adfae0588513a7635b725`  
		Last Modified: Thu, 17 Sep 2020 00:16:44 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d9c7a66fa3f8bda76123a4c1bdcb13a05ff5b8faf339e82a98184cb6fed45`  
		Last Modified: Thu, 17 Sep 2020 00:18:22 GMT  
		Size: 42.9 MB (42892005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603105aa4fcdc53b9a874455afd922c860f9c7aa6406530477812e4a2bbf210`  
		Last Modified: Thu, 17 Sep 2020 00:18:12 GMT  
		Size: 264.6 KB (264560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1833be1685f3348adcf20be665e1e9780399592e0db0aa57bdf164825fb590cb`  
		Last Modified: Thu, 17 Sep 2020 00:18:29 GMT  
		Size: 55.5 MB (55502394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:26fa4ea3b25c07b89debbec23d8475a2e81295e9a2c2f936611a9719390ecd03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.5 MB (324456036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d1bc4f8fbf31c2aa3f846ac05f0c9808d1ea1c9277494c97adeb8b38441c05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 23:17:57 GMT
ADD file:07638f480082d3760a79e7f8ab797a506252cc2233f89865558b0b5e0220a4d3 in / 
# Wed, 16 Sep 2020 23:18:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:18:02 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:18:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:18:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:49:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:50:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 00:50:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Sep 2020 00:50:03 GMT
ENV LANG=C.UTF-8
# Thu, 17 Sep 2020 00:50:04 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Sep 2020 00:50:06 GMT
ENV ROS_DISTRO=kinetic
# Thu, 17 Sep 2020 00:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:52:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 17 Sep 2020 00:52:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 00:52:59 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 00:53:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:54:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 00:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:72fb9e9daf6916d23d5ddb9755e3ab864abfa8ba4f352549179782677ea68012`  
		Last Modified: Fri, 04 Sep 2020 00:25:27 GMT  
		Size: 40.1 MB (40096941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899cdab0a82a447b311cc0646f11453c021df6968deccedf1187f915f1e8053b`  
		Last Modified: Wed, 16 Sep 2020 23:19:18 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016b9151e276d67695313eeb9bce429497ee8ab86848317064a39e8a8666c87a`  
		Last Modified: Wed, 16 Sep 2020 23:19:18 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727158034d7c22989558e6c5c700ff8c0e20942f6d4296293e5fd59e47f0cdc9`  
		Last Modified: Wed, 16 Sep 2020 23:19:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e073e177ffb2ca929b9b83efc7824b84c23b85434033f582dc27ac3eb5e88ad7`  
		Last Modified: Thu, 17 Sep 2020 02:25:28 GMT  
		Size: 4.8 MB (4819936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753b4dd9372d2e45878c50b980bbcf120893c7a734aa2b17adc8a314df9194b6`  
		Last Modified: Thu, 17 Sep 2020 02:25:27 GMT  
		Size: 14.7 KB (14746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd210d131ae0d1c1ac02e6a7c119d8f3ac82b889007270b8a86772383a4a8d2c`  
		Last Modified: Thu, 17 Sep 2020 02:25:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbfdda19cc98211de8b387744422a42fa50f25d8ee51810d3b1d9ccf82787e2`  
		Last Modified: Thu, 17 Sep 2020 02:27:28 GMT  
		Size: 176.0 MB (176006484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e22fd201597594e6d2073e0615524eac4a39e99166d6cc38bef74598960c4aa`  
		Last Modified: Thu, 17 Sep 2020 02:25:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e7cdc92ce708e8ff5e93a7ff775aec1ddeea7283ec0c6e3eaa43a572aeddfa`  
		Last Modified: Thu, 17 Sep 2020 02:27:51 GMT  
		Size: 46.0 MB (45952926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a8e48e259ed5433daf0059ecad65fef812c440696f575305baf297853673c2`  
		Last Modified: Thu, 17 Sep 2020 02:27:37 GMT  
		Size: 264.7 KB (264668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84e32e4d86ea7597e25bf4185855b7879d96cb392b68fed7d56d3156ddf930e`  
		Last Modified: Thu, 17 Sep 2020 02:28:01 GMT  
		Size: 57.3 MB (57298419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
