## `ros:eloquent-ros-base`

```console
$ docker pull ros@sha256:38e31f05534bba79981d6f3c737c14a4d4609849236efc1a046e866f9e046b14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:4d1c8c6e43052d8b5b2a19edc2b529d8516751aa207b27e6aaac045ff6d9bec7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.6 MB (283618004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ecd87ff213b37e8573826b7b3240a0902a6b57ff36675317f1fda6426dc8e57`
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
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:27:47 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 04:28:26 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:28:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:28:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:28:27 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:28:40 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42965efca798c9c9e706ab5922070f5654bcf4608d5190162edaac6d567628`  
		Last Modified: Thu, 16 Jan 2020 04:36:36 GMT  
		Size: 70.3 MB (70293967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea24eb1ad310cafced566a0eccc94ad52e979fa2bb226cc7897080d02ce0da2`  
		Last Modified: Thu, 16 Jan 2020 04:36:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f54fa04cfa49ffe305cc98e22817e1d7e10c1d05de2bad7b30572b4c15fb559`  
		Last Modified: Thu, 16 Jan 2020 04:36:42 GMT  
		Size: 4.6 MB (4602192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:af5c6862560a6933f018782114cb4ee51e36aec944444a7a89a5ec1966e26401
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237374716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62fe72b79d428c35d38291ea5ae7e7e3b0948f2530d6dac327d350b25c96788b`
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
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:15:34 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:17:25 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:17:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:17:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:17:31 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:18:06 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb05985b74964e9342cf7fea3660f7e829e196207602285054d94dbd52551db`  
		Last Modified: Thu, 16 Jan 2020 03:27:50 GMT  
		Size: 51.0 MB (51024178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfd7e9391f9003e2d47d56afbb32806f06263d0d3957ccfeefb70ca2644d0c3`  
		Last Modified: Thu, 16 Jan 2020 03:27:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055227d75c97e401b955db9ea1a4d784bf04b1926af6a84f351586a9b3a935f5`  
		Last Modified: Thu, 16 Jan 2020 03:27:59 GMT  
		Size: 3.5 MB (3516872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:94237ca5406272645d192a40267979829d49b6460a9ebf9ae72ad6fbdf55ac83
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257155305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0887f74845992d30957ff8706f1f8def1a9003e796f444350c68bf45a36c76`
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
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:08:05 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:10:24 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:10:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:10:50 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:11:37 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191819737b8386a2ca9385a20290b92b7398c773d5b1a91f628aec3b30d3dad`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 57.6 MB (57590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ac6d7be7b32161e12523997260627c3539594bf84bbd785783e640c63aac6`  
		Last Modified: Thu, 16 Jan 2020 03:22:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620498a630739d39314cb08eae34f29a33dd1e0b06483582035c8072e3fec4c9`  
		Last Modified: Thu, 16 Jan 2020 03:22:42 GMT  
		Size: 4.0 MB (3954504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
