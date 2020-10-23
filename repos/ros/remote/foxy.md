## `ros:foxy`

```console
$ docker pull ros@sha256:29a446118edb1287135489e1b210edfa035fa0565f5012e769dab7646c67d926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:d0286e3dcb16398cc667070851612faa241ab4e709236d4c640cac3edbefae74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231896384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359c2f755b5ac376c05f7d0b84cdf77cc62d840bee8435fdb26d37bdd39cec6f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:36:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:39:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:39:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 19:50:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 23 Oct 2020 19:50:28 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 19:50:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 19:50:29 GMT
ENV ROS_DISTRO=foxy
# Fri, 23 Oct 2020 19:51:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:51:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 23 Oct 2020 19:51:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 19:51:25 GMT
CMD ["bash"]
# Fri, 23 Oct 2020 19:52:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:52:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Oct 2020 19:52:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 23 Oct 2020 19:52:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff1f5aa6532e89f99088e3f051edc77e327f1be209cae1a67a9a4a9d75ab918`  
		Last Modified: Fri, 23 Oct 2020 19:57:00 GMT  
		Size: 1.2 MB (1176911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ea0b4003c131677032f1b780e81fe1340558bdda164da50e8dc00028e8fe99`  
		Last Modified: Fri, 23 Oct 2020 19:56:58 GMT  
		Size: 5.5 MB (5547520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff461b03c5c5f446813ac962f11e949edf73b550d9ae717ba14ba7ce61a8d38`  
		Last Modified: Fri, 23 Oct 2020 19:56:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460e0d4a81e4ebdf7a4c14e4bf2b9c72ca9b72cdf39de2719afa761c68aaf488`  
		Last Modified: Fri, 23 Oct 2020 20:00:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48b7fa4fb5e8e765240f8c252b65fdccd3685bdc69ccb934c0e426c8b97b4e4`  
		Last Modified: Fri, 23 Oct 2020 20:01:08 GMT  
		Size: 119.5 MB (119543305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3901dc9ae34a8fe67000daaeeff461a351f64030cf8e89f8296cf57f2bacff4f`  
		Last Modified: Fri, 23 Oct 2020 20:00:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caff70c4b06cafa0ce870f65534593a6abc812ff97a229d85fcae28574ee026`  
		Last Modified: Fri, 23 Oct 2020 20:01:27 GMT  
		Size: 66.6 MB (66584989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc255db0b796faec61ae3ce103a1ac10ba541c3e7a2f8b532082f4b72fa5817d`  
		Last Modified: Fri, 23 Oct 2020 20:01:14 GMT  
		Size: 198.9 KB (198937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a3fce668106b67e10bc56451c2a235c0111af32d5c28457c7a41902335e8e1`  
		Last Modified: Fri, 23 Oct 2020 20:01:14 GMT  
		Size: 2.0 KB (2022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799e6f44e37084af33cc067569f317ac64f610d950f388b03d123eda99e8d779`  
		Last Modified: Fri, 23 Oct 2020 20:01:18 GMT  
		Size: 10.3 MB (10281138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:995e65a35230e6805759b705444e83ee97d16cea069ef4b8ec2aa39e448b68e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208063287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e7f201abd60ac334c863e6cd48266cb37624eefb806f9fa38cb491221b2051`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:06:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:06:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:07:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 23 Oct 2020 19:17:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 23 Oct 2020 19:17:09 GMT
ENV LANG=C.UTF-8
# Fri, 23 Oct 2020 19:17:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 23 Oct 2020 19:17:10 GMT
ENV ROS_DISTRO=foxy
# Fri, 23 Oct 2020 19:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:18:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 23 Oct 2020 19:18:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 23 Oct 2020 19:18:50 GMT
CMD ["bash"]
# Fri, 23 Oct 2020 19:19:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:19:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 23 Oct 2020 19:19:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 23 Oct 2020 19:20:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a57a33cfa330c14ee308343f9e2a73382a99ccf08c3c905dbb22831ec69c86`  
		Last Modified: Fri, 23 Oct 2020 19:24:02 GMT  
		Size: 1.2 MB (1178042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c463e5d0fb6cd5bb763e1856a0ca0db13a28b7a5ff531cf5ea2a2d778ab6e536`  
		Last Modified: Fri, 23 Oct 2020 19:24:00 GMT  
		Size: 5.5 MB (5513934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7a377b36c34d24c6e2a5c5a7f9cbcfad3511145bdf413951e31feedfadd819`  
		Last Modified: Fri, 23 Oct 2020 19:23:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad05750da6711171d9e6bc951deb25363c73387191387317035493b2dfb906db`  
		Last Modified: Fri, 23 Oct 2020 19:28:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c43209a9b3b4bbf79d2cd4bec408b6a10896c0be489647abae660c22795be3`  
		Last Modified: Fri, 23 Oct 2020 19:28:39 GMT  
		Size: 103.7 MB (103745689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4fb66ec5b9b5757fd1a402e456f3491403f9ef7e1c8ee11acb75a5fdf904b0`  
		Last Modified: Fri, 23 Oct 2020 19:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddddfcb0393ae0fe369e29064ba409fe62bde765df1464793879f3410b4f316`  
		Last Modified: Fri, 23 Oct 2020 19:29:02 GMT  
		Size: 61.0 MB (60958911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6531033339e6393879238938148156d47dae8b45e1b3809a269556aa0cd59867`  
		Last Modified: Fri, 23 Oct 2020 19:28:48 GMT  
		Size: 199.0 KB (198997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfb1dfe89f61cf90c8bcd7798e60a1f13f22c321e2d356d80332b13a2b817df`  
		Last Modified: Fri, 23 Oct 2020 19:28:48 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4806f95eaa044ddf19f7f9a55a89b3b2cb41fe530f85578e18720e7e36a07a0d`  
		Last Modified: Fri, 23 Oct 2020 19:28:50 GMT  
		Size: 9.3 MB (9298933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
