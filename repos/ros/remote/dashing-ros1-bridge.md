## `ros:dashing-ros1-bridge`

```console
$ docker pull ros@sha256:e8161d75303e3f203342364d3559b6c5cec3b1049df754bfe14265a6bb792afa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:c27740dc93808d4644af7bebcc8fe0ddca92be1d3dbe2f533d3b1e86a115a560
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **418.5 MB (418497387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60a3d1963d419b15a9f23da630d35553668b728eadfb2f0da58fac7b5029b2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:26:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:24:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:24:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 01:45:28 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 17 Sep 2020 01:45:29 GMT
ENV LANG=C.UTF-8
# Thu, 17 Sep 2020 01:45:29 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Sep 2020 01:45:29 GMT
ENV ROS_DISTRO=dashing
# Thu, 17 Sep 2020 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:47:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 17 Sep 2020 01:47:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 01:47:27 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 01:48:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:48:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 01:48:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 17 Sep 2020 01:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:48:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 01:48:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Sep 2020 01:48:52 GMT
ENV ROS1_DISTRO=melodic
# Thu, 17 Sep 2020 01:48:52 GMT
ENV ROS2_DISTRO=dashing
# Thu, 17 Sep 2020 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:50:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.6-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:51:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:51:04 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5aab880c2f23fd5bf095a6e1a941ba3c3488993cfc6ee5357ef112834aa0f0e`  
		Last Modified: Thu, 17 Sep 2020 00:46:55 GMT  
		Size: 838.2 KB (838176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff46beebaffa079e954504803bc595a5f6e147a355f4dedc87f40f3af82541e6`  
		Last Modified: Thu, 17 Sep 2020 02:05:15 GMT  
		Size: 4.9 MB (4868515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f0e50c7d585ec379b79811c18fe858d1c056ff843ad99f5b83185707ea2c0`  
		Last Modified: Thu, 17 Sep 2020 02:05:14 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de63688b11552e31a081677d4f8cdec5298a10ec1d6aa5b1ddc9fb8b9e9aac3`  
		Last Modified: Thu, 17 Sep 2020 02:11:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee77e9c3f7390e8cc1b3e5e1fbfe31f13ad9e2af574a69d8b8abefbd9e7e0ac`  
		Last Modified: Thu, 17 Sep 2020 02:11:55 GMT  
		Size: 179.4 MB (179393476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f961fabbceff1d76e4305b1c6048337be354232737f97ccd151276da74f26e7`  
		Last Modified: Thu, 17 Sep 2020 02:11:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9cb2d87933e49c15eeeebe32d39cd5e8dcf84963da147f357cacaed4ff6096`  
		Last Modified: Thu, 17 Sep 2020 02:12:16 GMT  
		Size: 64.1 MB (64125632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b583f79a0bd0565b8b23d96cfbf1d02d4877720a5fe96e0ff0505fe881e2fc`  
		Last Modified: Thu, 17 Sep 2020 02:12:05 GMT  
		Size: 189.5 KB (189520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d334f1291e00addae04dcd53dbe2a5b6a7c2e0589390f526ccdebe2c85ee1b65`  
		Last Modified: Thu, 17 Sep 2020 02:12:05 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941cb035e0528e898f5053d856fdbabf27a3984d99d316fed7180889d0931ae`  
		Last Modified: Thu, 17 Sep 2020 02:12:06 GMT  
		Size: 4.3 MB (4312555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aac0a8fe3afab7b74ce7f8addcec2ee8736eaaeed13921b5704b49dd9e9668`  
		Last Modified: Thu, 17 Sep 2020 02:12:23 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce8b747454ce7b1b1bbe98187ed8d8c14061402d21cf744ce9e50506ebdf399`  
		Last Modified: Thu, 17 Sep 2020 02:12:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f950a80d5ba21059662ec26fe3015180498990e745c4cc6256923aa4720bdc`  
		Last Modified: Thu, 17 Sep 2020 02:12:51 GMT  
		Size: 117.6 MB (117639063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513a205d8118f0760826c4476cfbc0d674c287c6ca95915497fd2b113d2f2d2`  
		Last Modified: Thu, 17 Sep 2020 02:12:29 GMT  
		Size: 19.8 MB (19787027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2736739d35d3c9ae936f706f035c128c562a29978a7ffd5abba42a778ff593`  
		Last Modified: Thu, 17 Sep 2020 02:12:22 GMT  
		Size: 638.3 KB (638343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b3635037471e27585a66cbeef5680c2ea64ee7cee962cd201c8ad4ef4c91f0`  
		Last Modified: Thu, 17 Sep 2020 02:12:22 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:13679cf8c047d4ca7a74feace1f632312556ef3216dc16fbe8e4948bcaa13e2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.7 MB (354658434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adb8e980b844705c8b5ac4a240df44eb557862d4fb06f0f882ce5ccec8c863f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:28:20 GMT
ADD file:f239c31583452916dd5a653985cbb35d0acb5e97723cb8bcb089ab6dbc009543 in / 
# Wed, 16 Sep 2020 22:28:25 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:28:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:28:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:28:29 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:39:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:40:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:40:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 00:00:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 17 Sep 2020 00:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 17 Sep 2020 00:00:57 GMT
ENV LC_ALL=C.UTF-8
# Thu, 17 Sep 2020 00:00:58 GMT
ENV ROS_DISTRO=dashing
# Thu, 17 Sep 2020 00:03:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:03:34 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 17 Sep 2020 00:03:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 00:03:36 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 00:04:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:04:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 00:05:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 17 Sep 2020 00:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:05:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 00:05:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Sep 2020 00:05:36 GMT
ENV ROS1_DISTRO=melodic
# Thu, 17 Sep 2020 00:05:37 GMT
ENV ROS2_DISTRO=dashing
# Thu, 17 Sep 2020 00:07:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:08:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.6-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:08:31 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:46d8d5151783740c4f70c11c624110a72d6b7d8493331685c23eb44a666f962c`  
		Last Modified: Mon, 07 Sep 2020 15:50:39 GMT  
		Size: 22.3 MB (22279228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0959cf6d665929dbf2838b855f0075660add7f1c3faf5448a40700196e90b0`  
		Last Modified: Wed, 16 Sep 2020 22:30:31 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1764331539d248c00080a27564305167245f13addfdedad6507d51963b39257c`  
		Last Modified: Wed, 16 Sep 2020 22:30:31 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491b5d3c9f39553218974674ea250f3fb389092036ebb38a8af47267d5549cd1`  
		Last Modified: Thu, 17 Sep 2020 00:20:53 GMT  
		Size: 838.9 KB (838860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e462b6c5168c4d5a30db12ddc6821469b045aa66cc93b25d061dd70449178`  
		Last Modified: Thu, 17 Sep 2020 00:20:51 GMT  
		Size: 4.1 MB (4084274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84540db783e530a304a48855cbad8b87e5ff41c406ae1ddb38a585138a2174b`  
		Last Modified: Thu, 17 Sep 2020 00:20:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538b6d6c3d4e431168dc5b5efeff3a8eda16f5e3ee9af7c8e44b10151045dd4`  
		Last Modified: Thu, 17 Sep 2020 00:29:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82361440c49383572d5fd9aca178549e5b63bb8cc3a4feb0e3e92bf602d3b6`  
		Last Modified: Thu, 17 Sep 2020 00:30:04 GMT  
		Size: 153.5 MB (153526590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8032396274e0c0ef9c048b6232502e8ed81e462fa76b0c6a7360eb7e1178e4c4`  
		Last Modified: Thu, 17 Sep 2020 00:29:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074b4952c03ac28760edc4b41d3fc06a9e804311400808b14955c381c0847f3d`  
		Last Modified: Thu, 17 Sep 2020 00:30:26 GMT  
		Size: 48.5 MB (48528952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fdf2c24ac4abf7a83e5627ec6f8edacf05c8cf3aebd5fea194f6a9e6f55cd0`  
		Last Modified: Thu, 17 Sep 2020 00:30:12 GMT  
		Size: 189.6 KB (189572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579a5d7ae8f0c2d72806d4359e38be4f2168b0ee0bebd84064af1e53e270e824`  
		Last Modified: Thu, 17 Sep 2020 00:30:12 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964180e94dd6e5f33de9990268aaa73880ce491bc7d742be2e3a0476c354255`  
		Last Modified: Thu, 17 Sep 2020 00:30:13 GMT  
		Size: 3.2 MB (3248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a504227b8453594b7534a6ccbc0ff3b2320b55d55a1ee6b6267ddd29648eb31`  
		Last Modified: Thu, 17 Sep 2020 00:30:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59913fdf29caff4d1a251c3a620f41d6b711dcd64f58d04cf294b3146041b92c`  
		Last Modified: Thu, 17 Sep 2020 00:30:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f695287cacd5d493f77dbbf759e5a10bfa141b1b469b104e1c444f879b084f05`  
		Last Modified: Thu, 17 Sep 2020 00:31:13 GMT  
		Size: 110.5 MB (110520572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7185fc65241891f278b71ea4ca3c4475ff808f7f323f664b12b1283f2c406eb8`  
		Last Modified: Thu, 17 Sep 2020 00:30:39 GMT  
		Size: 10.8 MB (10801099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca3d517f486bddce7e2de352b8b3e78a3fa41bbb5fac830a84250efee95af6`  
		Last Modified: Thu, 17 Sep 2020 00:30:34 GMT  
		Size: 634.9 KB (634855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbff5c711eb9c60684f5520de78bffdbbc88f51243fa9dea36633319ae38099`  
		Last Modified: Thu, 17 Sep 2020 00:30:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:aa2a339382c4213072255a94d771fe9097d2c12c1e8272b8edeaf17096c4bf91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.0 MB (387009390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04895db9ae8c4880477877a1e2ce8e7b5d8d2bdca09e916956c81f987330b0a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:29:47 GMT
ADD file:b8316fc82a2cf230ce4af7dcf02ec1d7e56b156cf610af8ed23b64509c77c799 in / 
# Wed, 19 Aug 2020 21:29:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:29:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:29:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:29:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:14:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:14:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:15:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:35:47 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 19 Aug 2020 23:35:48 GMT
ENV LANG=C.UTF-8
# Wed, 19 Aug 2020 23:35:49 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 Aug 2020 23:35:50 GMT
ENV ROS_DISTRO=dashing
# Wed, 19 Aug 2020 23:37:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:37:58 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 19 Aug 2020 23:38:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 23:38:00 GMT
CMD ["bash"]
# Wed, 19 Aug 2020 23:39:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 19 Aug 2020 23:39:56 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 19 Aug 2020 23:40:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:40:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:40:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 Aug 2020 23:40:49 GMT
ENV ROS1_DISTRO=melodic
# Wed, 19 Aug 2020 23:40:50 GMT
ENV ROS2_DISTRO=dashing
# Tue, 01 Sep 2020 22:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 22:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.6-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 22:54:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 22:54:30 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:237528ba509b2abcdba1ff1344bab27ad56235cdb3c1c131d3587f6fba4d92c9`  
		Last Modified: Sat, 08 Aug 2020 00:25:26 GMT  
		Size: 23.7 MB (23721798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b96f31d8b2bf3ce9eb4ac49e6c7411defa4057c1791f02f54c14f2de298ec`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 35.2 KB (35203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82b0e39008d2fa246a0dca4cfa5feb15db58591582a839bd69d5000aa2e96d`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ca375b8d34c9bc764ae24791184cba22510f0c002815b4f9766dd0463f5f5e`  
		Last Modified: Wed, 19 Aug 2020 21:32:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f6dffa388a5afeaeeec2de7d9fa800e94f1e7f1ad2274f59f7157286f86ec`  
		Last Modified: Thu, 20 Aug 2020 00:06:26 GMT  
		Size: 838.7 KB (838677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed841649442752ce9cf01dc1412c51934d12d590691361fb31a442d8793944`  
		Last Modified: Thu, 20 Aug 2020 00:06:21 GMT  
		Size: 4.5 MB (4451831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0e3e7bfbdedb57d66e251fe599446189354d4603eb3d458f1fedb2de4c72a8`  
		Last Modified: Thu, 20 Aug 2020 00:06:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e79a72e11b6e2117dbd4dae2a4673f7d8d31a14a1cffa234bc1e6637f0659fd`  
		Last Modified: Thu, 20 Aug 2020 00:16:23 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28841f536a353faaa820c6564df2b33e24c29347a9d62487a056e888edbdc3ac`  
		Last Modified: Thu, 20 Aug 2020 00:17:12 GMT  
		Size: 165.1 MB (165076559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74784c24f72dee0be556cbb37b89c05ea077933a9a1a49c22fa4b610412f4bf`  
		Last Modified: Thu, 20 Aug 2020 00:16:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bd5e01cd95c97549278c1e5b3869eeab949f41aa237dfdde8b74f076557e55`  
		Last Modified: Thu, 20 Aug 2020 00:17:34 GMT  
		Size: 56.8 MB (56837310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b420753a6a76c91bfa50e2840570baf864542c60730406dde01622aaeb9ae986`  
		Last Modified: Thu, 20 Aug 2020 00:17:22 GMT  
		Size: 187.6 KB (187648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e032b1979cdde7985f06c7c76e74d8367956b47c5c225bbc06b4593bd0d750`  
		Last Modified: Thu, 20 Aug 2020 00:17:22 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a5266993a413241f868a142b60bc74e7d4603e5bef8cedf01dc98e142ac47`  
		Last Modified: Thu, 20 Aug 2020 00:17:22 GMT  
		Size: 3.7 MB (3664658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4097f75cf46de7ede04627453e7461dbc9086d3437f6c53de312ff24fb643c1`  
		Last Modified: Tue, 01 Sep 2020 23:14:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa47e9cabf4ba5369fed31153d5136c2cb6e1cedd7eb324b1de93cc68c3ee4b2`  
		Last Modified: Tue, 01 Sep 2020 23:14:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a669974be4907d90aa4d0795541923088504dca5e7234bd0cc461996a50372fe`  
		Last Modified: Tue, 01 Sep 2020 23:15:21 GMT  
		Size: 116.6 MB (116611981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f88cce6f92968a2fa5a40fa1cd986df5a42bd384f2774f9827e0ff14b2a6d5`  
		Last Modified: Tue, 01 Sep 2020 23:14:53 GMT  
		Size: 14.9 MB (14942394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a82e3da75169ab07fd55ce12644d4f7af0fc6e162dde0e23431ea5a871663`  
		Last Modified: Tue, 01 Sep 2020 23:14:44 GMT  
		Size: 635.8 KB (635754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cd6da70e0eeda7f722da7869b2c5cb81d8c967f8e7cc1a56d3db1bd562483b`  
		Last Modified: Tue, 01 Sep 2020 23:14:44 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
