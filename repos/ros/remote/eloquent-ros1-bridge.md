## `ros:eloquent-ros1-bridge`

```console
$ docker pull ros@sha256:dd971dbf6542094440a958a65bd19f555b35b911c389dd0673c0e65a0fabe0d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:ba9dd5ec8353e71b75523cb8f8270b3799b68c76c3f74c831feb2a2b0d5f5620
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423897708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:832292664c0f0178b1842eb746881c03bd5172869a0a876c21af72663cddf362`
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
# Thu, 17 Sep 2020 01:51:19 GMT
ENV ROS_DISTRO=eloquent
# Thu, 17 Sep 2020 01:52:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:52:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 17 Sep 2020 01:52:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 01:52:25 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 01:53:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:53:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 01:53:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 17 Sep 2020 01:53:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:53:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 01:53:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Sep 2020 01:53:33 GMT
ENV ROS1_DISTRO=melodic
# Thu, 17 Sep 2020 01:53:33 GMT
ENV ROS2_DISTRO=eloquent
# Thu, 17 Sep 2020 01:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:54:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:54:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:54:53 GMT
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
	-	`sha256:18c1bd5efbc47d70f96a44d4995492ee01e82dbce803fc3551930fa0dd58c959`  
		Last Modified: Thu, 17 Sep 2020 02:13:56 GMT  
		Size: 183.0 MB (182962582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d48d3ea10f1e617aa1466a998fbd119d353025c39c3071a66aa59465056f8b`  
		Last Modified: Thu, 17 Sep 2020 02:12:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44ac6505d2844ee8f42bba50b4d4000663223ead1402193f68a6f6e8512488`  
		Last Modified: Thu, 17 Sep 2020 02:14:16 GMT  
		Size: 63.5 MB (63506221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732711d58827a55d1d08e40a0f6ec9dbee46d71cec5ceca32f8d6fdca9db7c11`  
		Last Modified: Thu, 17 Sep 2020 02:14:05 GMT  
		Size: 188.2 KB (188195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf85c8f377a08783f01c3f460c5e69068ff3a1e6870e2947d7cb38a371e6b0`  
		Last Modified: Thu, 17 Sep 2020 02:14:05 GMT  
		Size: 2.0 KB (2018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186c1ba5a1d165786ce91c6e9458003311d8487cacfcba12415de43219f8d753`  
		Last Modified: Thu, 17 Sep 2020 02:14:07 GMT  
		Size: 4.6 MB (4580483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee04e434a08fedb87f93d423042bb678e511a5448a8904e5757fbb070e00d56`  
		Last Modified: Thu, 17 Sep 2020 02:14:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d19345896bf19729fd48db15b7738dcb2da194c8bbaa12a8d1c9d69079d537`  
		Last Modified: Thu, 17 Sep 2020 02:14:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3e7925613ece031ac05cbf70839822cecc3ba878331b2eb113b021e5d080b8`  
		Last Modified: Thu, 17 Sep 2020 02:14:50 GMT  
		Size: 117.6 MB (117647425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723a3ebc0a6417d2e6c1bbca801a5a11074f74c604c7ce916cf5cf2a5246d36f`  
		Last Modified: Thu, 17 Sep 2020 02:14:29 GMT  
		Size: 22.0 MB (21954581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6008f9a315e0e7d0851616d76f00cfd8bb95b4f3c47cdeaaa1f3903f5beede1`  
		Last Modified: Thu, 17 Sep 2020 02:14:21 GMT  
		Size: 646.4 KB (646430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1d41aaf03155d4e1bd554129789fdc6709e9e18b9ac511d2a3de9acd5e83b6`  
		Last Modified: Thu, 17 Sep 2020 02:14:21 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:cd9145e3ea4776570314c6bec8f437d626d9d21dc8163fa3278a02db47559e5d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.6 MB (359577025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73650078981a3a643c01b66647a4f690eb02ea99626b25022331fdb345d14784`
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
# Thu, 17 Sep 2020 00:08:49 GMT
ENV ROS_DISTRO=eloquent
# Thu, 17 Sep 2020 00:11:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:11:05 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 17 Sep 2020 00:11:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 17 Sep 2020 00:11:06 GMT
CMD ["bash"]
# Thu, 17 Sep 2020 00:12:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:12:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 17 Sep 2020 00:12:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 17 Sep 2020 00:12:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:12:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 17 Sep 2020 00:12:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 17 Sep 2020 00:13:00 GMT
ENV ROS1_DISTRO=melodic
# Thu, 17 Sep 2020 00:13:01 GMT
ENV ROS2_DISTRO=eloquent
# Thu, 17 Sep 2020 00:15:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:15:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:15:56 GMT
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
	-	`sha256:34437b0296d2cb41f47128a197101c072fdc7f2178bf5688f1e14273b540da25`  
		Last Modified: Thu, 17 Sep 2020 00:32:05 GMT  
		Size: 156.6 MB (156564716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52264f5d7d437cfeeee4846f8d46a4b62ee4a09ec523555b35a13dc6c851662`  
		Last Modified: Thu, 17 Sep 2020 00:31:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a71f50402b8ed4c3bc7e3d7ad60b42fb47f58d4fec40d46267b255fe3ccf559`  
		Last Modified: Thu, 17 Sep 2020 00:32:24 GMT  
		Size: 47.9 MB (47906781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad6f0a1cd11890a886b66346eb25d0ce30dad3ca2c60f5381e92543ebbf52fd`  
		Last Modified: Thu, 17 Sep 2020 00:32:12 GMT  
		Size: 188.3 KB (188262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e97ccc2f6957c0a60e3e74dc8e4f48a04ec8d96ce37288b4d95ca88fdd2b8c7`  
		Last Modified: Thu, 17 Sep 2020 00:32:12 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe75d1198bddcd4830c6efc985567b8109c1ce55c4ba1a37599ad6e2e5deafb`  
		Last Modified: Thu, 17 Sep 2020 00:32:14 GMT  
		Size: 3.5 MB (3492132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2231c53a89ed4e56ea1d5c2a7cf1c06f82cd8121b53247bdb489d7b30ec8325`  
		Last Modified: Thu, 17 Sep 2020 00:32:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fa13c7c022caa1473c56acdf1d74c98bdde4a3508af703ecb72071a395873f`  
		Last Modified: Thu, 17 Sep 2020 00:32:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1da8ba02a502f93a9521c449364eee67cdddbae57eff262d76e1571b94c7a60`  
		Last Modified: Thu, 17 Sep 2020 00:33:10 GMT  
		Size: 110.5 MB (110528858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1deb2aea192566e8845a0795e695f9bfd6197facf61e3d094baadad446d816`  
		Last Modified: Thu, 17 Sep 2020 00:32:39 GMT  
		Size: 13.0 MB (13045945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7571677c3395713ad1bd8c54fcf8a1d070400b9c18f4d81edb78ceab0a90292c`  
		Last Modified: Thu, 17 Sep 2020 00:32:34 GMT  
		Size: 642.5 KB (642453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f071e1749bf82781604232722d35df52307d9588497153f1d5d22f4aa61f6a`  
		Last Modified: Thu, 17 Sep 2020 00:32:33 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ba5cf5b77e9c3fd7d20c02be86a5b9b73e7571744445a7f2946d520229a28e46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.9 MB (391886298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db8e699eb94ae92a50f3e1ed642e8d514045e4664ddb63435332049058470b71`
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
# Wed, 19 Aug 2020 23:41:33 GMT
ENV ROS_DISTRO=eloquent
# Wed, 19 Aug 2020 23:43:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:43:56 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 19 Aug 2020 23:44:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 23:44:05 GMT
CMD ["bash"]
# Wed, 19 Aug 2020 23:45:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:45:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 19 Aug 2020 23:45:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 19 Aug 2020 23:45:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:46:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:46:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 Aug 2020 23:46:16 GMT
ENV ROS1_DISTRO=melodic
# Wed, 19 Aug 2020 23:46:17 GMT
ENV ROS2_DISTRO=eloquent
# Tue, 01 Sep 2020 22:59:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 23:00:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 23:01:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 23:02:08 GMT
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
	-	`sha256:8ec9ee67ebc7a9a3b1216eab5c4a345702e44eae7a9fff4fad12499effa8344a`  
		Last Modified: Thu, 20 Aug 2020 00:18:58 GMT  
		Size: 168.3 MB (168336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d75e28c8240dfc8949551ca4c1617e383db5d297829003ef5698019b624612`  
		Last Modified: Thu, 20 Aug 2020 00:17:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e0cdda8a34abe3bfa3b73536e0030455ae3e982acc73bf8c8e00e6d687282f`  
		Last Modified: Thu, 20 Aug 2020 00:19:55 GMT  
		Size: 56.2 MB (56215374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d21ffae48aa4b71b612738ef9b854d7feb25e121809c7d5f554b1f08518232b`  
		Last Modified: Thu, 20 Aug 2020 00:19:44 GMT  
		Size: 185.8 KB (185816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6e42893747fc9a2b9e3056d9b900532c86cee4b89b2e234485d61c71bdccf`  
		Last Modified: Thu, 20 Aug 2020 00:19:42 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31de7c457e7456398ebeb457b7c54fde0b41862ee09081b2c88665c2070d6e61`  
		Last Modified: Thu, 20 Aug 2020 00:19:45 GMT  
		Size: 3.9 MB (3931671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82af62f901f638748c341e5e64e1c2c85ead54fb6bf31e4dafc313c4554574c`  
		Last Modified: Tue, 01 Sep 2020 23:15:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3516ca37f10f68ff26fc2e70665ebce675a72e14389ed480fda5bdef08e87d`  
		Last Modified: Tue, 01 Sep 2020 23:15:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca8a2565d41351db2bba23f5333af2da9d23cf0bd02d2f3f4511ca4538a19b`  
		Last Modified: Tue, 01 Sep 2020 23:16:14 GMT  
		Size: 116.6 MB (116620587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a49b84e3a7bbef346c8709116aafa822a8567c1dadf30db086b72a6a11aede`  
		Last Modified: Tue, 01 Sep 2020 23:15:40 GMT  
		Size: 16.9 MB (16898812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb691d5ac27d131b13c4120af1bdf357048d5e18a9f39025e6689057084dd6e`  
		Last Modified: Tue, 01 Sep 2020 23:15:33 GMT  
		Size: 644.9 KB (644899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f887b7fbfad1ebd1f8ad2c2c5e485adf4b8afd64974cca08a9dfb0330a022a9a`  
		Last Modified: Tue, 01 Sep 2020 23:15:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
