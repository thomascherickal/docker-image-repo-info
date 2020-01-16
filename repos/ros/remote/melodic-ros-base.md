## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:380a4afed7c294394662de2cbda6757ceeba499c7ff5bd41a4c3f7bc41a91aa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:051d5af176ed91de0384f4524bf6820cc325f16e32fdbb9715f7e194b5ca3a6d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.4 MB (419369514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d421f8825627e33e65ea2376c6c0f66de4fafc713c1962d5913b8b1213fa58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:da9a0650f1934edcbe631a9baaf4c593eea71834706e18e8d6516714c7689823
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.2 MB (372195683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d091638dd04ba6737e13119939ad257b24a46d5d1ff83dd5755d3a6d33af7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8691bcd38f7325d3fbe8e7203842f40d0be8bb995e792e2a019bc964dfc49b90
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395828307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378a0887ed4c6132ad327ea544378650843be5227cf6037d80635b233556dae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
