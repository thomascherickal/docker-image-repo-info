## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:89bd2908aa0a085785b8b3d5a7688075908a73ecb5949427edef423c902cb11c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f64d667517d4194cc1cb5295c993bae5e45a4ddc81009009f098e59477b5947c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291831038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe585c03c1a96b54c22cea321c656f5a9ac16d39c5d2350cb8b8d1a9839f85b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 09:43:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:49:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:49:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 13:49:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 13:49:38 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 13:49:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 13:49:38 GMT
ENV ROS_DISTRO=melodic
# Fri, 12 Mar 2021 13:54:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:54:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 13:54:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 13:54:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ed3fdd01cb132a75576627b585cbad41af7070332373601bf156cf4196736`  
		Last Modified: Fri, 12 Mar 2021 10:19:48 GMT  
		Size: 841.3 KB (841338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e14253e5e1988d1da318161fcd62f7283c85a895d3290c387f20568717ed1a`  
		Last Modified: Fri, 12 Mar 2021 15:02:27 GMT  
		Size: 4.9 MB (4872989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72cfe4cc8a334266cf329ea82265f2fd5aba02064102886f265705a681ccdb1`  
		Last Modified: Fri, 12 Mar 2021 15:02:25 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932f904e0c2e5738177d4a07a3105883e3ba9121a06d166d647847a4162e7fbe`  
		Last Modified: Fri, 12 Mar 2021 15:02:25 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1068d361b0771d575c41a4f1169cb45f5a4a00fd93713e6a1f83d423662ac954`  
		Last Modified: Fri, 12 Mar 2021 15:03:29 GMT  
		Size: 259.4 MB (259403716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d312b43e68b363feabd281230d5bda0e2a77558352c25b251f0c01b4b0e04d`  
		Last Modified: Fri, 12 Mar 2021 15:02:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:0a8f331dd64fc7fa53f635e2935b9d6e887367827a2db9c70e7f15c7b3fca182
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.1 MB (266099714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53fd551d9210cd03bde2dc7cbe74fefb63774d9f934ce352bba471c1e583ee90`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 03:11:28 GMT
ADD file:40381fcd77266e4b2259c02af63359b9cff79b4908e5f800f2b3cb9c555e092c in / 
# Thu, 04 Mar 2021 03:11:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 03:11:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 03:11:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 03:11:35 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:03:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:03:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:03:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 04:04:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 04 Mar 2021 04:04:02 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 04:04:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 04:04:03 GMT
ENV ROS_DISTRO=melodic
# Thu, 04 Mar 2021 04:07:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:07:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 04 Mar 2021 04:07:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 04:07:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9ac910c0311f3581d0d4d512d5b9cb75f3cb4ac0ac05c27d5afe506d19ede5a4`  
		Last Modified: Mon, 01 Mar 2021 16:09:58 GMT  
		Size: 22.3 MB (22290308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b89a6b5bccf38a10ff30cb0b414a7e2dec5567d954850dfb98d67977e13fc38`  
		Last Modified: Thu, 04 Mar 2021 03:13:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36058ccabae5f30074009cee645af7e052db260738cc0bc08ec9386b0f8cf37e`  
		Last Modified: Thu, 04 Mar 2021 03:13:18 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055861ede19fe8606dca16da2271075d5d46ad1234acc782d134f1c941be2c72`  
		Last Modified: Thu, 04 Mar 2021 04:40:54 GMT  
		Size: 841.1 KB (841118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6fbf11975e6d976397a06700430b7ac889c14444fc7ad18a7be40983d9d468`  
		Last Modified: Thu, 04 Mar 2021 04:40:53 GMT  
		Size: 4.1 MB (4085567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e165c7fe50b6918ba96d9a80c7d25887947ae8b8aa8fd70fe773e79a745dff1b`  
		Last Modified: Thu, 04 Mar 2021 04:40:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66813ffd3dc90b1f26728f0e66d1c24cd6e2c2c078750cdc6f7697217303194b`  
		Last Modified: Thu, 04 Mar 2021 04:40:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dff8ede634e1a7e6011e2b2d50f4a3a848f1765210ce7b032a6b4b81e5aea3`  
		Last Modified: Thu, 04 Mar 2021 04:42:02 GMT  
		Size: 238.9 MB (238879846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37f78aee1fceb61306d380bf73d536b720d5026a0f8f760f84ba896d330705d`  
		Last Modified: Thu, 04 Mar 2021 04:40:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d7b787134646adce6e53304fb83fa8ad02903868f9e7b5b36ca1c3e8a9a6d6c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281345258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec28f77c9b76c72ba794b463149dda106810a96944c6a6795175123035b3655`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:12:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:13:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:13:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 03:13:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 04 Mar 2021 03:13:16 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 03:13:17 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 03:13:17 GMT
ENV ROS_DISTRO=melodic
# Thu, 04 Mar 2021 03:15:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:15:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 04 Mar 2021 03:15:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 03:15:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb395c83b2a400ee825ab384f2c51674c732ff599742e127b5639756b0cc7a8b`  
		Last Modified: Thu, 04 Mar 2021 04:00:41 GMT  
		Size: 840.9 KB (840907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3418e9c274d60c6f142b25861afead56aafa5ece244d451cab264c52961bc618`  
		Last Modified: Thu, 04 Mar 2021 04:00:40 GMT  
		Size: 4.5 MB (4453487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ee6263fb6dc4f04d5d149d5aa0d9932daea95f32e0478a12a5e66a986a1931`  
		Last Modified: Thu, 04 Mar 2021 04:00:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8e05aa8adaaca88884b382bafe4f0be06ae98213b2218241a2902c79e1cfee`  
		Last Modified: Thu, 04 Mar 2021 04:00:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555500c77492e3762a37fca4a8c00f0b77bbf70f9e460aa0dcfb94c4d8ecea80`  
		Last Modified: Thu, 04 Mar 2021 04:01:42 GMT  
		Size: 252.3 MB (252315934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2937675ccb8ca23fe751124dde72dbaaad5c4a092de0ffcc1b7af3b251b6572`  
		Last Modified: Thu, 04 Mar 2021 04:00:40 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
