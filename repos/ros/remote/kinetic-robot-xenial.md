## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:e301629503931be9cee6ce78419c14424eb9a5e6da6f8e5a9bf5ca3bb4523e2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:1888f434f114b4223ba9bda007bb7981cb4b68d704e195295dd56b86d82292e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.4 MB (379404126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2525150b447fbb2d6a543e27adc8745578789b26edd7a648165cf500364283ab`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 05:19:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:19:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 05:19:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 05:19:54 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 05:19:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 05:19:55 GMT
ENV ROS_DISTRO=kinetic
# Wed, 17 Jun 2020 05:22:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:22:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 05:22:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 05:22:10 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 05:22:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:22:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 05:23:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:23:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ac56f782e838259f8c19966a568bae9945419306e06dcc23cd0bec6f9123f1`  
		Last Modified: Wed, 17 Jun 2020 06:00:30 GMT  
		Size: 5.4 MB (5361853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f252d86210549455b146c498ded2c3accd8a9269b2ac72d802380b2dc35a76`  
		Last Modified: Wed, 17 Jun 2020 06:00:29 GMT  
		Size: 13.1 KB (13105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb88bb0196a765c25c05e35ec971e2e07c5a05e4e99db67ef1dd4da0d2d09cb`  
		Last Modified: Wed, 17 Jun 2020 06:00:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726771e90eff006799f01f17cf7cdc7335d31fa8b8a12b4f04e05aabd9cf3216`  
		Last Modified: Wed, 17 Jun 2020 06:01:15 GMT  
		Size: 187.1 MB (187138771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3c8419bbc4fea5dbe3787671e305e0aa761bd4e3837833661516dc60726046`  
		Last Modified: Wed, 17 Jun 2020 06:00:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e8ba19648919befd471811a35947cc5e234d0983ecec37101a718f22a0ff39`  
		Last Modified: Wed, 17 Jun 2020 06:01:33 GMT  
		Size: 57.2 MB (57240182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e7f002d7125f744928f400d26deb78c293b66900d24ef8c5549b781b7a2bc8`  
		Last Modified: Wed, 17 Jun 2020 06:01:21 GMT  
		Size: 258.0 KB (258016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8ef6189a4a3db6b199234b47c95f415ec83b2d8c91cb492426beeb77179caf`  
		Last Modified: Wed, 17 Jun 2020 06:01:36 GMT  
		Size: 63.6 MB (63572408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f64b42178d720e581faf229b7e8ea7f0ae12bfe178134e4192a66b310d02175`  
		Last Modified: Wed, 17 Jun 2020 06:01:47 GMT  
		Size: 21.5 MB (21497544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:3e9a5a68beb9611e1e6e128b591138d10da66592300ce96a5d2c3ab15f28d916
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330490838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf82b36103c544aa6a6b3c8612f2650398f25d402ced3e4638dba28675fecb08`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 02:04:31 GMT
ADD file:6cc12f5b0908f30b9097dd8947a769888e2fed5c2a25671d1e4cd93ac0ef7a2a in / 
# Wed, 17 Jun 2020 02:04:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:04:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 02:05:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 02:05:12 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:10:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:10:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:10:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 03:10:07 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:10:08 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:10:09 GMT
ENV ROS_DISTRO=kinetic
# Wed, 17 Jun 2020 03:13:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:13:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 03:13:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 03:13:18 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 03:14:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:14:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 03:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:16:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:964b1ad4ea33c6edf524b0fba723b83aa90e37a66419cf5e514392304bd73309`  
		Last Modified: Mon, 18 May 2020 15:50:57 GMT  
		Size: 39.0 MB (38964390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b1c0566b01f5b9247bdf23fee3adfd14071d248058523063939ce8c482863c`  
		Last Modified: Wed, 17 Jun 2020 02:05:52 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5534a4581c7bc4061f7f3c35130d6daa15345f5791fe5c4c90cbe06def252991`  
		Last Modified: Wed, 17 Jun 2020 02:05:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0db3772af551e10afa4bced33b87cf3a0716943e901e4a9da41b1caac84b55`  
		Last Modified: Wed, 17 Jun 2020 02:05:53 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b88d1e1f8eaab795890a44aba254120710460cd3c229c81d2cb305a5ef9c219`  
		Last Modified: Wed, 17 Jun 2020 03:52:39 GMT  
		Size: 4.6 MB (4614611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e8cecde1e2d564293841b0d9d6b26c76fa0aa603f9ad1883d43f11436879c0`  
		Last Modified: Wed, 17 Jun 2020 03:52:37 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9136828cd2351f794e02e625555b17588dbd52b1a4b35e3f7e26122b4d56aae9`  
		Last Modified: Wed, 17 Jun 2020 03:52:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0858d8df7908efcf17daa7a718f5ef97381d0c3faa4411b28faa8f71692d73ce`  
		Last Modified: Wed, 17 Jun 2020 03:53:36 GMT  
		Size: 168.0 MB (167990816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dac4d3368b30a5de5b79fd1b2be37bb3c6429704537df5b4d285d9d0e019172`  
		Last Modified: Wed, 17 Jun 2020 03:52:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07868dd899caa834aa89cbe99dbe455161839e250dc222109b94d7d8b9e4750`  
		Last Modified: Wed, 17 Jun 2020 03:53:58 GMT  
		Size: 42.9 MB (42891228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f65b34e704ea516b44679fd2cabb7606d59e98ddf086d3446a28de21d744d0`  
		Last Modified: Wed, 17 Jun 2020 03:53:44 GMT  
		Size: 258.0 KB (258033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c25b3453cfdf8cdb2a0e3128187e22f604c3076e4bd1b99ee7835fbdcf368`  
		Last Modified: Wed, 17 Jun 2020 03:53:59 GMT  
		Size: 55.5 MB (55499848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb57a2a0fe505fbbfd3993e3dd8917ff746d4e2fa7241f8a220acffe8d9aea69`  
		Last Modified: Wed, 17 Jun 2020 03:54:12 GMT  
		Size: 20.3 MB (20256859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5c0171cb9aec4a7d1169a96207ecc3a1874eb7d5019ed05098912e4369e05108
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344855922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088a637eb393bdb280c219c964eb1405ae41bdcb784cfd0851b004c827776161`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:33:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:33:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:33:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 03:33:33 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:33:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:33:34 GMT
ENV ROS_DISTRO=kinetic
# Wed, 17 Jun 2020 03:36:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:36:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 03:36:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 03:36:44 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 03:37:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:38:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 03:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:41:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74cff2b55cc1ac6f7ad4718e83136db9dec33c5be38c87a928aa36bbfde7566`  
		Last Modified: Wed, 17 Jun 2020 04:33:21 GMT  
		Size: 4.8 MB (4819796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f4d034fcebccfa995aa3aa1d01b86cc2c73ea51b080c83877d4414643fbb55`  
		Last Modified: Wed, 17 Jun 2020 04:33:18 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105a0776d9d3f152933f93de729ae98cbeac2d0061b5c733ded7f5a77ab741b2`  
		Last Modified: Wed, 17 Jun 2020 04:33:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9316d6685dc45d027e52b671446b511e3debca2bccdee58a14225227f480385`  
		Last Modified: Wed, 17 Jun 2020 04:34:25 GMT  
		Size: 176.0 MB (176005103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7200b7aee2230d09ff1dabc93fc086026bf1a3a3017c3e11c11b245ae887606`  
		Last Modified: Wed, 17 Jun 2020 04:33:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4349463016054a81234bcfadcb190da3b5988ac06d0f72fd1588e878a152d9c7`  
		Last Modified: Wed, 17 Jun 2020 04:34:43 GMT  
		Size: 46.0 MB (45952479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c135de60033d097437ffdb1e337581bae8dcb477be92c12aca095203748fc64`  
		Last Modified: Wed, 17 Jun 2020 04:34:32 GMT  
		Size: 258.1 KB (258074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6014cbe345e2855aaf3b358d8c7547c4b95d0bc0561938d7c3a10aed4fce3d`  
		Last Modified: Wed, 17 Jun 2020 04:34:47 GMT  
		Size: 57.3 MB (57285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104fd2a768b12c3d8a7c63eae7eb4885489e1d74d2b539166740a6cfbb88f6fa`  
		Last Modified: Wed, 17 Jun 2020 04:35:07 GMT  
		Size: 20.5 MB (20516104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
