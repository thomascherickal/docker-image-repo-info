## `ros:rolling`

```console
$ docker pull ros@sha256:1fa55af3acfd7b9e2753fde9d5e5953eea19c2bb63c13d5777e0d8406fabc422
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0ca440b04ee9a577030af329f7674c8d991944ab81828b85359eddeacb9bf5a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207796945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b4cee9c8e38a4aee1ea49eb1f23d690d539a407032cf3e248da8423c8fb31cb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:43:22 GMT
ADD file:6d1bd041dcbfb2d51c871c8eb820202f5597b37ac4e4b94ce976fbc157619c8e in / 
# Wed, 17 Jun 2020 01:43:25 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:43:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:43:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:43:33 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:58:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:58:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 04:25:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 04:25:44 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 04:25:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Jul 2020 18:43:37 GMT
ENV ROS_DISTRO=rolling
# Wed, 01 Jul 2020 18:45:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.1-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jul 2020 18:45:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 01 Jul 2020 18:45:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Jul 2020 18:45:48 GMT
CMD ["bash"]
# Wed, 01 Jul 2020 18:46:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jul 2020 18:46:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Jul 2020 18:46:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Jul 2020 18:47:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.1-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63de6a4b0fc89f1aa36d95a840e6729cca22d2abaa887bfaf634c40ad4560ed4`  
		Last Modified: Sun, 07 Jun 2020 08:26:19 GMT  
		Size: 27.2 MB (27159755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243514e240f4c2654743395ffa5aed01b5eaf985f0118cdb2089629e0e9747d8`  
		Last Modified: Wed, 17 Jun 2020 01:45:14 GMT  
		Size: 32.3 KB (32336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ba51c40fb5f743fb4a4050b63644e7727c21a1cffba4c4767ac41118ac6d3`  
		Last Modified: Wed, 17 Jun 2020 01:45:14 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684e0fb606a03cddd5fc30fb6aee6055e851951eff13e4859295a3097063bba7`  
		Last Modified: Wed, 17 Jun 2020 01:45:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7becc6ba0698cca4766101c1e07007231a2bbad3952ec0c01c4706b5dc09c`  
		Last Modified: Wed, 17 Jun 2020 04:40:14 GMT  
		Size: 1.2 MB (1175791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ab96636dc90f9fea2726c2bf53a0f70a76853a496b08e0f3420bb95ef55dea`  
		Last Modified: Wed, 17 Jun 2020 04:40:13 GMT  
		Size: 5.5 MB (5516600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da0b15f3c3835f213d1d6997096f6e6d9cf7b0bcd50604bcca3b1575907e09`  
		Last Modified: Wed, 17 Jun 2020 04:40:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449fc159008401ac37e72ba47ebe0af89cd7453d6fba04661d8bd4f84e9e77d5`  
		Last Modified: Wed, 17 Jun 2020 04:48:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388b599c1990dab1639e9556f54ab4759ff1c6b7573c60cb3db5746e00441998`  
		Last Modified: Wed, 01 Jul 2020 18:51:22 GMT  
		Size: 103.5 MB (103494211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d02007c5c211609c2dac229b372b2cf831434e3ae1841ab61c09c08d46a077`  
		Last Modified: Wed, 01 Jul 2020 18:50:49 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d8457f00e69b3504803d27bdffc888edc7fca2beccdcb3b5fd9918da3b80e1`  
		Last Modified: Wed, 01 Jul 2020 18:51:46 GMT  
		Size: 60.9 MB (60929037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82001e5bb8ea47219c856938ca8d67f524f1461bf4f193743e5053d78514fd57`  
		Last Modified: Wed, 01 Jul 2020 18:51:28 GMT  
		Size: 182.2 KB (182205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f0080a5aedebd8b2823beb4f050bbb4f3ee06896024f6692db8e80d4fe31dd`  
		Last Modified: Wed, 01 Jul 2020 18:51:28 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d911e759060c7825f89b461b5ef1b5a5b095008eca02edc6da191b6d631265`  
		Last Modified: Wed, 01 Jul 2020 18:51:32 GMT  
		Size: 9.3 MB (9302086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
