<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:dashing`](#rosdashing)
-	[`ros:dashing-ros-base`](#rosdashing-ros-base)
-	[`ros:dashing-ros-base-bionic`](#rosdashing-ros-base-bionic)
-	[`ros:dashing-ros-core`](#rosdashing-ros-core)
-	[`ros:dashing-ros-core-bionic`](#rosdashing-ros-core-bionic)
-	[`ros:eloquent`](#roseloquent)
-	[`ros:eloquent-ros-base`](#roseloquent-ros-base)
-	[`ros:eloquent-ros-base-bionic`](#roseloquent-ros-base-bionic)
-	[`ros:eloquent-ros-core`](#roseloquent-ros-core)
-	[`ros:eloquent-ros-core-bionic`](#roseloquent-ros-core-bionic)
-	[`ros:kinetic`](#roskinetic)
-	[`ros:kinetic-perception`](#roskinetic-perception)
-	[`ros:kinetic-perception-xenial`](#roskinetic-perception-xenial)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-robot-xenial`](#roskinetic-robot-xenial)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic-ros-base-xenial`](#roskinetic-ros-base-xenial)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-core-xenial`](#roskinetic-ros-core-xenial)
-	[`ros:latest`](#roslatest)
-	[`ros:melodic`](#rosmelodic)
-	[`ros:melodic-perception`](#rosmelodic-perception)
-	[`ros:melodic-perception-bionic`](#rosmelodic-perception-bionic)
-	[`ros:melodic-perception-stretch`](#rosmelodic-perception-stretch)
-	[`ros:melodic-robot`](#rosmelodic-robot)
-	[`ros:melodic-robot-bionic`](#rosmelodic-robot-bionic)
-	[`ros:melodic-robot-stretch`](#rosmelodic-robot-stretch)
-	[`ros:melodic-ros-base`](#rosmelodic-ros-base)
-	[`ros:melodic-ros-base-bionic`](#rosmelodic-ros-base-bionic)
-	[`ros:melodic-ros-base-stretch`](#rosmelodic-ros-base-stretch)
-	[`ros:melodic-ros-core`](#rosmelodic-ros-core)
-	[`ros:melodic-ros-core-bionic`](#rosmelodic-ros-core-bionic)
-	[`ros:melodic-ros-core-stretch`](#rosmelodic-ros-core-stretch)

## `ros:dashing`

```console
$ docker pull ros@sha256:af5a737150f0672d2d0c7c9c7ab70c928832bfaccf43be427a09291daa82547b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing` - linux; amd64

```console
$ docker pull ros@sha256:b796c14ea663537129897769aa6c715a851ca08dffd4875ef2ecaa31a4dbd431
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (281049542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ed091d2d46225c6d99f54047f0e0a8fc6516e21075a7671cf8a56c6863443f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV ROS_DISTRO=dashing
# Sat, 22 Feb 2020 00:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:46:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:46:11 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:46:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:46:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:46:54 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:47:14 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a948b279d83acfa13fc8ba206da3da7e40ed19b8915f1aaaba599979d17519f`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 431.2 KB (431215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a68418cfe6a1da2b80130ce9f6eba94beac90ecd22c560138b35fcf1a0d5a90`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9448a84bb86ed570f856fc1cef1c23716fc8b0ba031aa63710f06e8aff498b10`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 207.9 KB (207889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1049f6fef203479acfba1c05e8b6190faa348b5eb82de5e124372d8fabc1cc57`  
		Last Modified: Sat, 22 Feb 2020 00:54:32 GMT  
		Size: 68.1 MB (68088474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da4046905a2b449e59ee9d90a7eb8b9d0005b3de43ec964b3ae05fc2308434`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6942dd9597559007e2591b9bc9c5996a4a898b4facd096145243b5e5cba8d37d`  
		Last Modified: Sat, 22 Feb 2020 00:54:46 GMT  
		Size: 4.3 MB (4340323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm variant v7

```console
$ docker pull ros@sha256:1ef60ada30f85cd6700ce44bc06ef788df48959b6febe65816286e17958bf64e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.3 MB (235265957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3796b8ccbe7ae74b731ef4e88158e7da7360610b22925af427d58d2f462747`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:49:09 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 22:49:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:49:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:49:35 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:51:15 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:51:18 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:51:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:51:21 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:51:57 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc228f61b9a73e78088e575985fad147d213afa62e6cfad76a07e579ea0eb13b`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 429.8 KB (429808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e586f5d1e985eb5e07d390e9b213e277ca150f22222e32c3c357f4a7f42fe22`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 1.9 KB (1905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13523ecae6c9b3ce4e218c043da5defad9be19749cdc06cffdd6ba23f66ff5c7`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 208.1 KB (208089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c19412f11f19cfd43d01ac4999ddecdae0e426d864db542aaf7f66a356b2f`  
		Last Modified: Fri, 21 Feb 2020 23:03:13 GMT  
		Size: 49.3 MB (49261529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf8db0ea13d86e0242057ab143cf0b39443c852ba671f6f2f6f354ab7899a96`  
		Last Modified: Fri, 21 Feb 2020 23:02:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae3c9123f169c24bb2d94b375c48462720f9f4266202108cad179d02fbce45d`  
		Last Modified: Fri, 21 Feb 2020 23:03:40 GMT  
		Size: 3.3 MB (3277650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e02847acf1e31743c169746d534b28afa214172e17f78ff0285576a5ddb14c55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254758785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3313edb0cd975007393c673fa24c126bcd4295cb0bc14c782b80dca4aed39698`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:34:34 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 23:34:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:35:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:35:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:36:32 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:36:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:36:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:36:47 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:37:28 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82df4c5f22c0fb4a2d7f6a4051dad1f9be0815a9b485614eaab5f64e367c425`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 429.8 KB (429799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c7996a80ba90618164151c7207be827adfb9555b606c66347222004bbf9a7`  
		Last Modified: Fri, 21 Feb 2020 23:48:09 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fdfb2846bf2beee368b2c4596dfc6a2f7e49aedfb76d763a7a0f60ff6a54b`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 208.2 KB (208172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e20c3397ce01be2c8ebc3d8b9ec521a8060dc633960093fd618208980f757`  
		Last Modified: Fri, 21 Feb 2020 23:48:30 GMT  
		Size: 55.6 MB (55560485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf2d06299030ad963e8cc03908a1728af04232b1574617be5a1c205662ce28f`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c8bb333639c06f7a1f171983a1301385b231d8cc6b5752a6825fa84a08158`  
		Last Modified: Fri, 21 Feb 2020 23:48:57 GMT  
		Size: 3.7 MB (3692372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base`

```console
$ docker pull ros@sha256:af5a737150f0672d2d0c7c9c7ab70c928832bfaccf43be427a09291daa82547b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b796c14ea663537129897769aa6c715a851ca08dffd4875ef2ecaa31a4dbd431
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (281049542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ed091d2d46225c6d99f54047f0e0a8fc6516e21075a7671cf8a56c6863443f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV ROS_DISTRO=dashing
# Sat, 22 Feb 2020 00:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:46:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:46:11 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:46:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:46:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:46:54 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:47:14 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a948b279d83acfa13fc8ba206da3da7e40ed19b8915f1aaaba599979d17519f`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 431.2 KB (431215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a68418cfe6a1da2b80130ce9f6eba94beac90ecd22c560138b35fcf1a0d5a90`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9448a84bb86ed570f856fc1cef1c23716fc8b0ba031aa63710f06e8aff498b10`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 207.9 KB (207889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1049f6fef203479acfba1c05e8b6190faa348b5eb82de5e124372d8fabc1cc57`  
		Last Modified: Sat, 22 Feb 2020 00:54:32 GMT  
		Size: 68.1 MB (68088474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da4046905a2b449e59ee9d90a7eb8b9d0005b3de43ec964b3ae05fc2308434`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6942dd9597559007e2591b9bc9c5996a4a898b4facd096145243b5e5cba8d37d`  
		Last Modified: Sat, 22 Feb 2020 00:54:46 GMT  
		Size: 4.3 MB (4340323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:1ef60ada30f85cd6700ce44bc06ef788df48959b6febe65816286e17958bf64e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.3 MB (235265957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3796b8ccbe7ae74b731ef4e88158e7da7360610b22925af427d58d2f462747`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:49:09 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 22:49:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:49:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:49:35 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:51:15 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:51:18 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:51:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:51:21 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:51:57 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc228f61b9a73e78088e575985fad147d213afa62e6cfad76a07e579ea0eb13b`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 429.8 KB (429808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e586f5d1e985eb5e07d390e9b213e277ca150f22222e32c3c357f4a7f42fe22`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 1.9 KB (1905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13523ecae6c9b3ce4e218c043da5defad9be19749cdc06cffdd6ba23f66ff5c7`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 208.1 KB (208089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c19412f11f19cfd43d01ac4999ddecdae0e426d864db542aaf7f66a356b2f`  
		Last Modified: Fri, 21 Feb 2020 23:03:13 GMT  
		Size: 49.3 MB (49261529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf8db0ea13d86e0242057ab143cf0b39443c852ba671f6f2f6f354ab7899a96`  
		Last Modified: Fri, 21 Feb 2020 23:02:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae3c9123f169c24bb2d94b375c48462720f9f4266202108cad179d02fbce45d`  
		Last Modified: Fri, 21 Feb 2020 23:03:40 GMT  
		Size: 3.3 MB (3277650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e02847acf1e31743c169746d534b28afa214172e17f78ff0285576a5ddb14c55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254758785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3313edb0cd975007393c673fa24c126bcd4295cb0bc14c782b80dca4aed39698`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:34:34 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 23:34:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:35:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:35:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:36:32 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:36:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:36:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:36:47 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:37:28 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82df4c5f22c0fb4a2d7f6a4051dad1f9be0815a9b485614eaab5f64e367c425`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 429.8 KB (429799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c7996a80ba90618164151c7207be827adfb9555b606c66347222004bbf9a7`  
		Last Modified: Fri, 21 Feb 2020 23:48:09 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fdfb2846bf2beee368b2c4596dfc6a2f7e49aedfb76d763a7a0f60ff6a54b`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 208.2 KB (208172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e20c3397ce01be2c8ebc3d8b9ec521a8060dc633960093fd618208980f757`  
		Last Modified: Fri, 21 Feb 2020 23:48:30 GMT  
		Size: 55.6 MB (55560485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf2d06299030ad963e8cc03908a1728af04232b1574617be5a1c205662ce28f`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c8bb333639c06f7a1f171983a1301385b231d8cc6b5752a6825fa84a08158`  
		Last Modified: Fri, 21 Feb 2020 23:48:57 GMT  
		Size: 3.7 MB (3692372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base-bionic`

```console
$ docker pull ros@sha256:af5a737150f0672d2d0c7c9c7ab70c928832bfaccf43be427a09291daa82547b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b796c14ea663537129897769aa6c715a851ca08dffd4875ef2ecaa31a4dbd431
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (281049542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ed091d2d46225c6d99f54047f0e0a8fc6516e21075a7671cf8a56c6863443f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV ROS_DISTRO=dashing
# Sat, 22 Feb 2020 00:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:46:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:46:11 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:46:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:46:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:46:54 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:47:14 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a948b279d83acfa13fc8ba206da3da7e40ed19b8915f1aaaba599979d17519f`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 431.2 KB (431215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a68418cfe6a1da2b80130ce9f6eba94beac90ecd22c560138b35fcf1a0d5a90`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9448a84bb86ed570f856fc1cef1c23716fc8b0ba031aa63710f06e8aff498b10`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 207.9 KB (207889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1049f6fef203479acfba1c05e8b6190faa348b5eb82de5e124372d8fabc1cc57`  
		Last Modified: Sat, 22 Feb 2020 00:54:32 GMT  
		Size: 68.1 MB (68088474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da4046905a2b449e59ee9d90a7eb8b9d0005b3de43ec964b3ae05fc2308434`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6942dd9597559007e2591b9bc9c5996a4a898b4facd096145243b5e5cba8d37d`  
		Last Modified: Sat, 22 Feb 2020 00:54:46 GMT  
		Size: 4.3 MB (4340323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:1ef60ada30f85cd6700ce44bc06ef788df48959b6febe65816286e17958bf64e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.3 MB (235265957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3796b8ccbe7ae74b731ef4e88158e7da7360610b22925af427d58d2f462747`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:49:09 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 22:49:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:49:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:49:35 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:51:15 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:51:18 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:51:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:51:21 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:51:57 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc228f61b9a73e78088e575985fad147d213afa62e6cfad76a07e579ea0eb13b`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 429.8 KB (429808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e586f5d1e985eb5e07d390e9b213e277ca150f22222e32c3c357f4a7f42fe22`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 1.9 KB (1905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13523ecae6c9b3ce4e218c043da5defad9be19749cdc06cffdd6ba23f66ff5c7`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 208.1 KB (208089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c19412f11f19cfd43d01ac4999ddecdae0e426d864db542aaf7f66a356b2f`  
		Last Modified: Fri, 21 Feb 2020 23:03:13 GMT  
		Size: 49.3 MB (49261529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf8db0ea13d86e0242057ab143cf0b39443c852ba671f6f2f6f354ab7899a96`  
		Last Modified: Fri, 21 Feb 2020 23:02:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae3c9123f169c24bb2d94b375c48462720f9f4266202108cad179d02fbce45d`  
		Last Modified: Fri, 21 Feb 2020 23:03:40 GMT  
		Size: 3.3 MB (3277650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e02847acf1e31743c169746d534b28afa214172e17f78ff0285576a5ddb14c55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254758785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3313edb0cd975007393c673fa24c126bcd4295cb0bc14c782b80dca4aed39698`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:34:34 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 23:34:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:35:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:35:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:36:32 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:36:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:36:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:36:47 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:37:28 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82df4c5f22c0fb4a2d7f6a4051dad1f9be0815a9b485614eaab5f64e367c425`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 429.8 KB (429799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c7996a80ba90618164151c7207be827adfb9555b606c66347222004bbf9a7`  
		Last Modified: Fri, 21 Feb 2020 23:48:09 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fdfb2846bf2beee368b2c4596dfc6a2f7e49aedfb76d763a7a0f60ff6a54b`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 208.2 KB (208172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e20c3397ce01be2c8ebc3d8b9ec521a8060dc633960093fd618208980f757`  
		Last Modified: Fri, 21 Feb 2020 23:48:30 GMT  
		Size: 55.6 MB (55560485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf2d06299030ad963e8cc03908a1728af04232b1574617be5a1c205662ce28f`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c8bb333639c06f7a1f171983a1301385b231d8cc6b5752a6825fa84a08158`  
		Last Modified: Fri, 21 Feb 2020 23:48:57 GMT  
		Size: 3.7 MB (3692372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core`

```console
$ docker pull ros@sha256:281973e5f260e460aa7d70220d178a2ef7ce109c193f93bd7d67f4d2564c1a7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5cb1a827dadeb3680689ad012c85b7dfd30c3bcb90783072ae0bf04056013abf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.7 MB (276709219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5bf8f53d79642893a8d4bc21d0e94515279baf28111fdbd67ee77525dacfb6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV ROS_DISTRO=dashing
# Sat, 22 Feb 2020 00:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:46:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:46:11 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:46:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:46:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:46:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a948b279d83acfa13fc8ba206da3da7e40ed19b8915f1aaaba599979d17519f`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 431.2 KB (431215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a68418cfe6a1da2b80130ce9f6eba94beac90ecd22c560138b35fcf1a0d5a90`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9448a84bb86ed570f856fc1cef1c23716fc8b0ba031aa63710f06e8aff498b10`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 207.9 KB (207889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1049f6fef203479acfba1c05e8b6190faa348b5eb82de5e124372d8fabc1cc57`  
		Last Modified: Sat, 22 Feb 2020 00:54:32 GMT  
		Size: 68.1 MB (68088474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da4046905a2b449e59ee9d90a7eb8b9d0005b3de43ec964b3ae05fc2308434`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:57026a7940bab8c308cd137364cd064c63065cb18ae4f3f335e82481fa2684e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.0 MB (231988307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abed97c2198a8c9467b62fc53fb5d8c86ffffac3729867f4e6683ae27ef89bd1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:49:09 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 22:49:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:49:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:49:35 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:51:15 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:51:18 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:51:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:51:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc228f61b9a73e78088e575985fad147d213afa62e6cfad76a07e579ea0eb13b`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 429.8 KB (429808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e586f5d1e985eb5e07d390e9b213e277ca150f22222e32c3c357f4a7f42fe22`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 1.9 KB (1905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13523ecae6c9b3ce4e218c043da5defad9be19749cdc06cffdd6ba23f66ff5c7`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 208.1 KB (208089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c19412f11f19cfd43d01ac4999ddecdae0e426d864db542aaf7f66a356b2f`  
		Last Modified: Fri, 21 Feb 2020 23:03:13 GMT  
		Size: 49.3 MB (49261529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf8db0ea13d86e0242057ab143cf0b39443c852ba671f6f2f6f354ab7899a96`  
		Last Modified: Fri, 21 Feb 2020 23:02:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:10f15e1da6a1bd7ea0bad5777e80e8a7aa87f1a434b4529bb1a939c12fde3d26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.1 MB (251066413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e731a59bd276dbd127ade924ebc42ced600927ccd0c9280a37e8c3aad2bc8416`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:34:34 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 23:34:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:35:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:35:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:36:32 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:36:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:36:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:36:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82df4c5f22c0fb4a2d7f6a4051dad1f9be0815a9b485614eaab5f64e367c425`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 429.8 KB (429799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c7996a80ba90618164151c7207be827adfb9555b606c66347222004bbf9a7`  
		Last Modified: Fri, 21 Feb 2020 23:48:09 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fdfb2846bf2beee368b2c4596dfc6a2f7e49aedfb76d763a7a0f60ff6a54b`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 208.2 KB (208172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e20c3397ce01be2c8ebc3d8b9ec521a8060dc633960093fd618208980f757`  
		Last Modified: Fri, 21 Feb 2020 23:48:30 GMT  
		Size: 55.6 MB (55560485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf2d06299030ad963e8cc03908a1728af04232b1574617be5a1c205662ce28f`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core-bionic`

```console
$ docker pull ros@sha256:281973e5f260e460aa7d70220d178a2ef7ce109c193f93bd7d67f4d2564c1a7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:5cb1a827dadeb3680689ad012c85b7dfd30c3bcb90783072ae0bf04056013abf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.7 MB (276709219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5bf8f53d79642893a8d4bc21d0e94515279baf28111fdbd67ee77525dacfb6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV ROS_DISTRO=dashing
# Sat, 22 Feb 2020 00:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:46:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:46:11 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:46:54 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:46:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:46:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a948b279d83acfa13fc8ba206da3da7e40ed19b8915f1aaaba599979d17519f`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 431.2 KB (431215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a68418cfe6a1da2b80130ce9f6eba94beac90ecd22c560138b35fcf1a0d5a90`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9448a84bb86ed570f856fc1cef1c23716fc8b0ba031aa63710f06e8aff498b10`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 207.9 KB (207889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1049f6fef203479acfba1c05e8b6190faa348b5eb82de5e124372d8fabc1cc57`  
		Last Modified: Sat, 22 Feb 2020 00:54:32 GMT  
		Size: 68.1 MB (68088474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da4046905a2b449e59ee9d90a7eb8b9d0005b3de43ec964b3ae05fc2308434`  
		Last Modified: Sat, 22 Feb 2020 00:54:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:57026a7940bab8c308cd137364cd064c63065cb18ae4f3f335e82481fa2684e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.0 MB (231988307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abed97c2198a8c9467b62fc53fb5d8c86ffffac3729867f4e6683ae27ef89bd1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:49:09 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 22:49:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:49:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:49:35 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:51:15 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:51:18 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:51:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:51:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc228f61b9a73e78088e575985fad147d213afa62e6cfad76a07e579ea0eb13b`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 429.8 KB (429808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e586f5d1e985eb5e07d390e9b213e277ca150f22222e32c3c357f4a7f42fe22`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 1.9 KB (1905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13523ecae6c9b3ce4e218c043da5defad9be19749cdc06cffdd6ba23f66ff5c7`  
		Last Modified: Fri, 21 Feb 2020 23:02:53 GMT  
		Size: 208.1 KB (208089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c19412f11f19cfd43d01ac4999ddecdae0e426d864db542aaf7f66a356b2f`  
		Last Modified: Fri, 21 Feb 2020 23:03:13 GMT  
		Size: 49.3 MB (49261529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf8db0ea13d86e0242057ab143cf0b39443c852ba671f6f2f6f354ab7899a96`  
		Last Modified: Fri, 21 Feb 2020 23:02:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:10f15e1da6a1bd7ea0bad5777e80e8a7aa87f1a434b4529bb1a939c12fde3d26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.1 MB (251066413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e731a59bd276dbd127ade924ebc42ced600927ccd0c9280a37e8c3aad2bc8416`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:34:34 GMT
ENV ROS_DISTRO=dashing
# Fri, 21 Feb 2020 23:34:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:35:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:35:06 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:36:32 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:36:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:36:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:36:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82df4c5f22c0fb4a2d7f6a4051dad1f9be0815a9b485614eaab5f64e367c425`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 429.8 KB (429799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c7996a80ba90618164151c7207be827adfb9555b606c66347222004bbf9a7`  
		Last Modified: Fri, 21 Feb 2020 23:48:09 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fdfb2846bf2beee368b2c4596dfc6a2f7e49aedfb76d763a7a0f60ff6a54b`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 208.2 KB (208172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e20c3397ce01be2c8ebc3d8b9ec521a8060dc633960093fd618208980f757`  
		Last Modified: Fri, 21 Feb 2020 23:48:30 GMT  
		Size: 55.6 MB (55560485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf2d06299030ad963e8cc03908a1728af04232b1574617be5a1c205662ce28f`  
		Last Modified: Fri, 21 Feb 2020 23:48:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent`

```console
$ docker pull ros@sha256:880957eb44e6a0f18d965203ab8f31109927877c4bf23791b20dcb46aa6ffd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent` - linux; amd64

```console
$ docker pull ros@sha256:77eccd0b6ce36bd3018094f4e0c8b9418d35ac4ecfc55dc48d408278a3c3a0a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283520543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91508ca0535cfb7da1c0f88d1894c119cbef780e38d9bd94038c445b7fb0b406`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:47:18 GMT
ENV ROS_DISTRO=eloquent
# Sat, 22 Feb 2020 00:47:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:47:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:47:33 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:48:11 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:48:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:48:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:48:12 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:48:29 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b83760638ae6f2143db8648a7c92a844b47bb873594399bc20b6375c44c7b`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 431.2 KB (431210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124f37844464555d0c94391dc7110178ab70200eb2f08ea894c050d8d1c0ae7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bfde953dd2e815d0a5cdf9b41354ee1d042aadf3ac078fb91114abea10e195`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 207.9 KB (207880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b30ce52367ec58066394e8e27c0b9d7d7fd7e5fa5af56f2a592a257403aa34`  
		Last Modified: Sat, 22 Feb 2020 00:55:12 GMT  
		Size: 70.3 MB (70296629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b94a85b2460065ed2dab8fb076195022dc065c492f07191d2335d5b8ed4c7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a3f7006123954038fea264761122de129d9f97bcae6c9178059c77c1e6ea8`  
		Last Modified: Sat, 22 Feb 2020 00:55:18 GMT  
		Size: 4.6 MB (4603147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm variant v7

```console
$ docker pull ros@sha256:3ffc1de27ce3aabc3819f37627275aa91f0ca7c7dda9639e9296f63c7667b22d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237272358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751c0875af9f0f4e4e87df70bb51225e562a5c16b868fec4d9872cdd44e65c7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:52:05 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 22:52:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:52:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:52:30 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:53:51 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:53:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:53:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:53:55 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:54:23 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e62cdefc5bf78c9602a57479c10ce469d05b802e3025b71b4846bbcd62602`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 429.8 KB (429803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c9450f3685b6f4031b6400ae4869abd268966d337b2ad7663773dc4615496a`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e07bedb17d9459542bbaa99de7fc9721b641813fee5932a174006e2f20b04`  
		Last Modified: Fri, 21 Feb 2020 23:03:49 GMT  
		Size: 208.1 KB (208111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1699fcfc035b984ac79831ab2a6d20ec7b0fa65564008b212e553a25bf115c0c`  
		Last Modified: Fri, 21 Feb 2020 23:04:09 GMT  
		Size: 51.0 MB (51028905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694db7cc23ff163fd039767ffe17aa114ab77d1149dd5e5ade9e33c841b37c87`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23f38d15750f052846e0a60602265614caf188b56f1b97ab46bd907f5b5eb13`  
		Last Modified: Fri, 21 Feb 2020 23:04:19 GMT  
		Size: 3.5 MB (3516666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e68d469ee2cac92b4f412c224de222bd05b2bf37fcf39c815cada016dfcb78b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257058861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055b56b794cd9fee6633759e311637e7cf52ed3d4fb4052a085a362294c01856`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:37:39 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 23:38:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:38:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:38:17 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:39:50 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:39:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:39:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:39:56 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:40:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145391f2f629875b1fca7741ec8701d86f9caab78614468dec6ad11bb27a192a`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 429.8 KB (429807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34744fe6cdefc249c10c14b6f56762b4f4ed35010c992270823fcdc6d2f1e179`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0203544be95dcd8bfee7c584c574e44556aeb6f9a8a42851ff810a552d32c`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 208.2 KB (208162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656760554510f95cce9b5260e2787d84fe4a4f80758214822bc76a564c893f73`  
		Last Modified: Fri, 21 Feb 2020 23:49:30 GMT  
		Size: 57.6 MB (57597501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac7e83b90fd3748ccfd7072c4be8743c764ef914c3be98075659ad673075eb`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc5a6b81bb1b6013a11049ee388e06f80f98fee37e9b14fa3806960437e4436`  
		Last Modified: Fri, 21 Feb 2020 23:49:39 GMT  
		Size: 4.0 MB (3955436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-base`

```console
$ docker pull ros@sha256:880957eb44e6a0f18d965203ab8f31109927877c4bf23791b20dcb46aa6ffd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:77eccd0b6ce36bd3018094f4e0c8b9418d35ac4ecfc55dc48d408278a3c3a0a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283520543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91508ca0535cfb7da1c0f88d1894c119cbef780e38d9bd94038c445b7fb0b406`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:47:18 GMT
ENV ROS_DISTRO=eloquent
# Sat, 22 Feb 2020 00:47:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:47:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:47:33 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:48:11 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:48:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:48:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:48:12 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:48:29 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b83760638ae6f2143db8648a7c92a844b47bb873594399bc20b6375c44c7b`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 431.2 KB (431210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124f37844464555d0c94391dc7110178ab70200eb2f08ea894c050d8d1c0ae7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bfde953dd2e815d0a5cdf9b41354ee1d042aadf3ac078fb91114abea10e195`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 207.9 KB (207880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b30ce52367ec58066394e8e27c0b9d7d7fd7e5fa5af56f2a592a257403aa34`  
		Last Modified: Sat, 22 Feb 2020 00:55:12 GMT  
		Size: 70.3 MB (70296629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b94a85b2460065ed2dab8fb076195022dc065c492f07191d2335d5b8ed4c7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a3f7006123954038fea264761122de129d9f97bcae6c9178059c77c1e6ea8`  
		Last Modified: Sat, 22 Feb 2020 00:55:18 GMT  
		Size: 4.6 MB (4603147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:3ffc1de27ce3aabc3819f37627275aa91f0ca7c7dda9639e9296f63c7667b22d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237272358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751c0875af9f0f4e4e87df70bb51225e562a5c16b868fec4d9872cdd44e65c7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:52:05 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 22:52:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:52:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:52:30 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:53:51 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:53:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:53:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:53:55 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:54:23 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e62cdefc5bf78c9602a57479c10ce469d05b802e3025b71b4846bbcd62602`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 429.8 KB (429803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c9450f3685b6f4031b6400ae4869abd268966d337b2ad7663773dc4615496a`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e07bedb17d9459542bbaa99de7fc9721b641813fee5932a174006e2f20b04`  
		Last Modified: Fri, 21 Feb 2020 23:03:49 GMT  
		Size: 208.1 KB (208111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1699fcfc035b984ac79831ab2a6d20ec7b0fa65564008b212e553a25bf115c0c`  
		Last Modified: Fri, 21 Feb 2020 23:04:09 GMT  
		Size: 51.0 MB (51028905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694db7cc23ff163fd039767ffe17aa114ab77d1149dd5e5ade9e33c841b37c87`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23f38d15750f052846e0a60602265614caf188b56f1b97ab46bd907f5b5eb13`  
		Last Modified: Fri, 21 Feb 2020 23:04:19 GMT  
		Size: 3.5 MB (3516666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e68d469ee2cac92b4f412c224de222bd05b2bf37fcf39c815cada016dfcb78b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257058861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055b56b794cd9fee6633759e311637e7cf52ed3d4fb4052a085a362294c01856`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:37:39 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 23:38:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:38:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:38:17 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:39:50 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:39:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:39:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:39:56 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:40:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145391f2f629875b1fca7741ec8701d86f9caab78614468dec6ad11bb27a192a`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 429.8 KB (429807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34744fe6cdefc249c10c14b6f56762b4f4ed35010c992270823fcdc6d2f1e179`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0203544be95dcd8bfee7c584c574e44556aeb6f9a8a42851ff810a552d32c`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 208.2 KB (208162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656760554510f95cce9b5260e2787d84fe4a4f80758214822bc76a564c893f73`  
		Last Modified: Fri, 21 Feb 2020 23:49:30 GMT  
		Size: 57.6 MB (57597501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac7e83b90fd3748ccfd7072c4be8743c764ef914c3be98075659ad673075eb`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc5a6b81bb1b6013a11049ee388e06f80f98fee37e9b14fa3806960437e4436`  
		Last Modified: Fri, 21 Feb 2020 23:49:39 GMT  
		Size: 4.0 MB (3955436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-base-bionic`

```console
$ docker pull ros@sha256:880957eb44e6a0f18d965203ab8f31109927877c4bf23791b20dcb46aa6ffd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:77eccd0b6ce36bd3018094f4e0c8b9418d35ac4ecfc55dc48d408278a3c3a0a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283520543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91508ca0535cfb7da1c0f88d1894c119cbef780e38d9bd94038c445b7fb0b406`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:47:18 GMT
ENV ROS_DISTRO=eloquent
# Sat, 22 Feb 2020 00:47:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:47:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:47:33 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:48:11 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:48:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:48:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:48:12 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:48:29 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b83760638ae6f2143db8648a7c92a844b47bb873594399bc20b6375c44c7b`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 431.2 KB (431210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124f37844464555d0c94391dc7110178ab70200eb2f08ea894c050d8d1c0ae7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bfde953dd2e815d0a5cdf9b41354ee1d042aadf3ac078fb91114abea10e195`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 207.9 KB (207880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b30ce52367ec58066394e8e27c0b9d7d7fd7e5fa5af56f2a592a257403aa34`  
		Last Modified: Sat, 22 Feb 2020 00:55:12 GMT  
		Size: 70.3 MB (70296629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b94a85b2460065ed2dab8fb076195022dc065c492f07191d2335d5b8ed4c7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a3f7006123954038fea264761122de129d9f97bcae6c9178059c77c1e6ea8`  
		Last Modified: Sat, 22 Feb 2020 00:55:18 GMT  
		Size: 4.6 MB (4603147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3ffc1de27ce3aabc3819f37627275aa91f0ca7c7dda9639e9296f63c7667b22d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237272358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751c0875af9f0f4e4e87df70bb51225e562a5c16b868fec4d9872cdd44e65c7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:52:05 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 22:52:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:52:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:52:30 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:53:51 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:53:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:53:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:53:55 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:54:23 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e62cdefc5bf78c9602a57479c10ce469d05b802e3025b71b4846bbcd62602`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 429.8 KB (429803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c9450f3685b6f4031b6400ae4869abd268966d337b2ad7663773dc4615496a`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e07bedb17d9459542bbaa99de7fc9721b641813fee5932a174006e2f20b04`  
		Last Modified: Fri, 21 Feb 2020 23:03:49 GMT  
		Size: 208.1 KB (208111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1699fcfc035b984ac79831ab2a6d20ec7b0fa65564008b212e553a25bf115c0c`  
		Last Modified: Fri, 21 Feb 2020 23:04:09 GMT  
		Size: 51.0 MB (51028905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694db7cc23ff163fd039767ffe17aa114ab77d1149dd5e5ade9e33c841b37c87`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23f38d15750f052846e0a60602265614caf188b56f1b97ab46bd907f5b5eb13`  
		Last Modified: Fri, 21 Feb 2020 23:04:19 GMT  
		Size: 3.5 MB (3516666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e68d469ee2cac92b4f412c224de222bd05b2bf37fcf39c815cada016dfcb78b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257058861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055b56b794cd9fee6633759e311637e7cf52ed3d4fb4052a085a362294c01856`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:37:39 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 23:38:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:38:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:38:17 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:39:50 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:39:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:39:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:39:56 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:40:28 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145391f2f629875b1fca7741ec8701d86f9caab78614468dec6ad11bb27a192a`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 429.8 KB (429807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34744fe6cdefc249c10c14b6f56762b4f4ed35010c992270823fcdc6d2f1e179`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0203544be95dcd8bfee7c584c574e44556aeb6f9a8a42851ff810a552d32c`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 208.2 KB (208162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656760554510f95cce9b5260e2787d84fe4a4f80758214822bc76a564c893f73`  
		Last Modified: Fri, 21 Feb 2020 23:49:30 GMT  
		Size: 57.6 MB (57597501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac7e83b90fd3748ccfd7072c4be8743c764ef914c3be98075659ad673075eb`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc5a6b81bb1b6013a11049ee388e06f80f98fee37e9b14fa3806960437e4436`  
		Last Modified: Fri, 21 Feb 2020 23:49:39 GMT  
		Size: 4.0 MB (3955436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-core`

```console
$ docker pull ros@sha256:d118caa1963863805ee918e2505f305e98d0ec4327a5dc9b48a36c9adaa78958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:d7ac07810a09e4ea29a3d7c9d488a2874178c4ee68d54dbfbe70dfa67d315ae1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.9 MB (278917396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7392569736fcab77656545e701efd3dcaa2cb747045c7ea0416cffb4fbe595a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:47:18 GMT
ENV ROS_DISTRO=eloquent
# Sat, 22 Feb 2020 00:47:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:47:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:47:33 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:48:11 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:48:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:48:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:48:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b83760638ae6f2143db8648a7c92a844b47bb873594399bc20b6375c44c7b`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 431.2 KB (431210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124f37844464555d0c94391dc7110178ab70200eb2f08ea894c050d8d1c0ae7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bfde953dd2e815d0a5cdf9b41354ee1d042aadf3ac078fb91114abea10e195`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 207.9 KB (207880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b30ce52367ec58066394e8e27c0b9d7d7fd7e5fa5af56f2a592a257403aa34`  
		Last Modified: Sat, 22 Feb 2020 00:55:12 GMT  
		Size: 70.3 MB (70296629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b94a85b2460065ed2dab8fb076195022dc065c492f07191d2335d5b8ed4c7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:1cbb2981698844e2c3c194af0735b4095ff6e7bafb1d9f9ded08540024ea28a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233755692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03caeaf6cacf5322e37eb0b1fa88db788677c4a09ea0d4fe57fbee17fdf26a3a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:52:05 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 22:52:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:52:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:52:30 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:53:51 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:53:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:53:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:53:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e62cdefc5bf78c9602a57479c10ce469d05b802e3025b71b4846bbcd62602`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 429.8 KB (429803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c9450f3685b6f4031b6400ae4869abd268966d337b2ad7663773dc4615496a`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e07bedb17d9459542bbaa99de7fc9721b641813fee5932a174006e2f20b04`  
		Last Modified: Fri, 21 Feb 2020 23:03:49 GMT  
		Size: 208.1 KB (208111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1699fcfc035b984ac79831ab2a6d20ec7b0fa65564008b212e553a25bf115c0c`  
		Last Modified: Fri, 21 Feb 2020 23:04:09 GMT  
		Size: 51.0 MB (51028905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694db7cc23ff163fd039767ffe17aa114ab77d1149dd5e5ade9e33c841b37c87`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:712d5be51297cddff2bda9ae190106e0d3dd3c0054b87bba4e3e1741334812cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.1 MB (253103425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e03539e02d9b90fd7184c1eec6b541122acf9e0c13ccb8c291dfb916e62a8444`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:37:39 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 23:38:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:38:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:38:17 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:39:50 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:39:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:39:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:39:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145391f2f629875b1fca7741ec8701d86f9caab78614468dec6ad11bb27a192a`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 429.8 KB (429807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34744fe6cdefc249c10c14b6f56762b4f4ed35010c992270823fcdc6d2f1e179`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0203544be95dcd8bfee7c584c574e44556aeb6f9a8a42851ff810a552d32c`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 208.2 KB (208162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656760554510f95cce9b5260e2787d84fe4a4f80758214822bc76a564c893f73`  
		Last Modified: Fri, 21 Feb 2020 23:49:30 GMT  
		Size: 57.6 MB (57597501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac7e83b90fd3748ccfd7072c4be8743c764ef914c3be98075659ad673075eb`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-core-bionic`

```console
$ docker pull ros@sha256:d118caa1963863805ee918e2505f305e98d0ec4327a5dc9b48a36c9adaa78958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:d7ac07810a09e4ea29a3d7c9d488a2874178c4ee68d54dbfbe70dfa67d315ae1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.9 MB (278917396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7392569736fcab77656545e701efd3dcaa2cb747045c7ea0416cffb4fbe595a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:21 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:45:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 22 Feb 2020 00:45:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:45:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:47:18 GMT
ENV ROS_DISTRO=eloquent
# Sat, 22 Feb 2020 00:47:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:47:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 22 Feb 2020 00:47:33 GMT
RUN pip3 install -U     argcomplete
# Sat, 22 Feb 2020 00:48:11 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:48:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 22 Feb 2020 00:48:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:48:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da966be4a5099d61ead50dae69ffda05b90d272819d01c77cf0097c0e5606dd`  
		Last Modified: Sat, 22 Feb 2020 00:54:38 GMT  
		Size: 152.0 MB (152015601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3928787e8e1be86d8fe671227cf4f3820d04eacaac3455ff12ba5e7a6cd0727`  
		Last Modified: Sat, 22 Feb 2020 00:54:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c2c32b925d8251fdfb81071414186ff0cfe58b7a7c4a40c6819887f73ea508`  
		Last Modified: Sat, 22 Feb 2020 00:54:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70c1a6759a69c6bdacdc8d0e9e2adc2a19e3f1efe646b2c04a6d19a7679b31`  
		Last Modified: Sat, 22 Feb 2020 00:54:18 GMT  
		Size: 28.4 MB (28395722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b83760638ae6f2143db8648a7c92a844b47bb873594399bc20b6375c44c7b`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 431.2 KB (431210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124f37844464555d0c94391dc7110178ab70200eb2f08ea894c050d8d1c0ae7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bfde953dd2e815d0a5cdf9b41354ee1d042aadf3ac078fb91114abea10e195`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 207.9 KB (207880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b30ce52367ec58066394e8e27c0b9d7d7fd7e5fa5af56f2a592a257403aa34`  
		Last Modified: Sat, 22 Feb 2020 00:55:12 GMT  
		Size: 70.3 MB (70296629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b94a85b2460065ed2dab8fb076195022dc065c492f07191d2335d5b8ed4c7`  
		Last Modified: Sat, 22 Feb 2020 00:54:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:1cbb2981698844e2c3c194af0735b4095ff6e7bafb1d9f9ded08540024ea28a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233755692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03caeaf6cacf5322e37eb0b1fa88db788677c4a09ea0d4fe57fbee17fdf26a3a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:47:57 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:48:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 22:49:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:49:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:52:05 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 22:52:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:52:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 22:52:30 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 22:53:51 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:53:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 22:53:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:53:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5d8ad0470cc0da41ae5f0f48462ab292e750c6357adc668ac3e0b72e0b0e75`  
		Last Modified: Fri, 21 Feb 2020 23:03:30 GMT  
		Size: 133.6 MB (133567881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51b40381f7c57eb48f4c7680ceed8fd1cb86e6e1c827ae7ee0cdd194362704`  
		Last Modified: Fri, 21 Feb 2020 23:02:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f2ef24fd75d1e785fc5b15916673b7f3bb246e8c910607bc1fb6671032f58d`  
		Last Modified: Fri, 21 Feb 2020 23:02:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705414e608e99036e1a63bb9111cbf2a4fec5cdfd21141f9dd2726561c36802`  
		Last Modified: Fri, 21 Feb 2020 23:03:04 GMT  
		Size: 25.4 MB (25367051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e62cdefc5bf78c9602a57479c10ce469d05b802e3025b71b4846bbcd62602`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 429.8 KB (429803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c9450f3685b6f4031b6400ae4869abd268966d337b2ad7663773dc4615496a`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e07bedb17d9459542bbaa99de7fc9721b641813fee5932a174006e2f20b04`  
		Last Modified: Fri, 21 Feb 2020 23:03:49 GMT  
		Size: 208.1 KB (208111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1699fcfc035b984ac79831ab2a6d20ec7b0fa65564008b212e553a25bf115c0c`  
		Last Modified: Fri, 21 Feb 2020 23:04:09 GMT  
		Size: 51.0 MB (51028905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694db7cc23ff163fd039767ffe17aa114ab77d1149dd5e5ade9e33c841b37c87`  
		Last Modified: Fri, 21 Feb 2020 23:03:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:712d5be51297cddff2bda9ae190106e0d3dd3c0054b87bba4e3e1741334812cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.1 MB (253103425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e03539e02d9b90fd7184c1eec6b541122acf9e0c13ccb8c291dfb916e62a8444`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:16 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:33:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:33:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 21 Feb 2020 23:34:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:34:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:34:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:37:39 GMT
ENV ROS_DISTRO=eloquent
# Fri, 21 Feb 2020 23:38:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:38:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 21 Feb 2020 23:38:17 GMT
RUN pip3 install -U     argcomplete
# Fri, 21 Feb 2020 23:39:50 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:39:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 21 Feb 2020 23:39:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:39:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d73493808ce6f6f7d45ca5fb1333b3ce950d0cdc1640ccca46fc16f60570abd`  
		Last Modified: Fri, 21 Feb 2020 23:48:48 GMT  
		Size: 143.2 MB (143187904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282fd2aa8436bc43624281f20dcf830dccd5351b5be9efd46c8159cbf8ae0bef`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f7023ae98237ea9145a2625fa0cf720c553c89bdcd208a4646a65c5ca8efd`  
		Last Modified: Fri, 21 Feb 2020 23:48:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bff3fa4bbcab602445ad3a933a89124fd887b628dfab15441b44295988c55`  
		Last Modified: Fri, 21 Feb 2020 23:48:19 GMT  
		Size: 27.1 MB (27080861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145391f2f629875b1fca7741ec8701d86f9caab78614468dec6ad11bb27a192a`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 429.8 KB (429807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34744fe6cdefc249c10c14b6f56762b4f4ed35010c992270823fcdc6d2f1e179`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0203544be95dcd8bfee7c584c574e44556aeb6f9a8a42851ff810a552d32c`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 208.2 KB (208162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656760554510f95cce9b5260e2787d84fe4a4f80758214822bc76a564c893f73`  
		Last Modified: Fri, 21 Feb 2020 23:49:30 GMT  
		Size: 57.6 MB (57597501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac7e83b90fd3748ccfd7072c4be8743c764ef914c3be98075659ad673075eb`  
		Last Modified: Fri, 21 Feb 2020 23:49:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic`

```console
$ docker pull ros@sha256:43d5ae157fc3c46f526b61b9c335c8eaedab78ff7ae20133b49891ffa61655bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:2c075fb5be70e13dc96f087bc8eabe5cc64ee18a83982d780349c632d764476f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385441592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738ea393ac21a38436e6806c253439219c1b8c0161723043e806862701336b4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3d718acd020242cba3e9a740e208ed095982711260c1e6a13693983cbfec4b45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336674606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57c3d3fb765b350d8332a08950d3d91a4f41e9e12043026591b4e851388f1e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fd760e573470a83df7e3d09b1e370fe5f39339eda7d4d53773184969536db6cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350490262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0ce788fbb9d15d7ba91bff960b7f189d2f043949d8b424aa0fe3c7d34fc9ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:d7ec01863e0a3a05414a970ea60539531e196e7938f524962c5b891c53488d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:f6f27b7beb6659cf491a1c734f2a2b68a8ea9fa11bf9e589e87b464b9dcdf730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.9 MB (725867513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2cbe085d6ba013573114f53c8e9a93ba68812e57c625dc005c3b0df752e8d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:36 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727c79ea040f26770a21d33ddd52e20efcd96f4c9e2f97ed33c9c7a6f95583d7`  
		Last Modified: Sat, 22 Feb 2020 00:51:15 GMT  
		Size: 340.4 MB (340425921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:affef6df5bff26f5591a6bfcf0312394659d80609ecf450306ac86bec51cd750
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.2 MB (617197283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cddba418d7392655233163a0d375f45946231e7124cd5392de6df2863bdbb8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:34:27 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0f05f8c00e923c3366c8424a5474bac300e17b34d266c011666fedd7f9f23`  
		Last Modified: Fri, 21 Feb 2020 22:58:09 GMT  
		Size: 280.5 MB (280522677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:92a6dcf7929f3fedb02a688c4f80332717782380f286eeedbfe695f486004483
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.5 MB (641452392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbd5475a62a799f8a4c13f0bf1cf1036cb28f78e487531a41c6f5273661efc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:47 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5525c9121c3bf41c88ba09803955018eaf6fa451d354dc51e025b6fcaec53b1a`  
		Last Modified: Fri, 21 Feb 2020 23:44:18 GMT  
		Size: 291.0 MB (290962130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:d7ec01863e0a3a05414a970ea60539531e196e7938f524962c5b891c53488d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:f6f27b7beb6659cf491a1c734f2a2b68a8ea9fa11bf9e589e87b464b9dcdf730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.9 MB (725867513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2cbe085d6ba013573114f53c8e9a93ba68812e57c625dc005c3b0df752e8d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:36 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727c79ea040f26770a21d33ddd52e20efcd96f4c9e2f97ed33c9c7a6f95583d7`  
		Last Modified: Sat, 22 Feb 2020 00:51:15 GMT  
		Size: 340.4 MB (340425921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:affef6df5bff26f5591a6bfcf0312394659d80609ecf450306ac86bec51cd750
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.2 MB (617197283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cddba418d7392655233163a0d375f45946231e7124cd5392de6df2863bdbb8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:34:27 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0f05f8c00e923c3366c8424a5474bac300e17b34d266c011666fedd7f9f23`  
		Last Modified: Fri, 21 Feb 2020 22:58:09 GMT  
		Size: 280.5 MB (280522677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:92a6dcf7929f3fedb02a688c4f80332717782380f286eeedbfe695f486004483
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.5 MB (641452392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbd5475a62a799f8a4c13f0bf1cf1036cb28f78e487531a41c6f5273661efc6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:47 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5525c9121c3bf41c88ba09803955018eaf6fa451d354dc51e025b6fcaec53b1a`  
		Last Modified: Fri, 21 Feb 2020 23:44:18 GMT  
		Size: 291.0 MB (290962130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:fbb8763abcae1e23ebe2c4880f58a79a3c4782d5e82058d20d4ce3afb4e3c3e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:fc0fc6e27f939bbb8646cc906093cd28af2464673e1934e396365aa65c189eee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.2 MB (407205343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dad2b7cfd1c067a7254860051e5ba0c55032189a5019e3462beb2506a6de516`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:31:19 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8562cbcf9ab94f660f9ad756b3a323a24935a76950d87a81926201a133ae301f`  
		Last Modified: Sat, 22 Feb 2020 00:50:01 GMT  
		Size: 21.8 MB (21763751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:ec4e3aa73bf7b7f43ea433e778f5c36e1c190eb75dad41255c24dc82350afb6e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.7 MB (356714093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe58cf9ef47a1a053baa3228b26b3d29424475418e52557ca50877cbe73db89a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:29:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56cde4cae5f9a17754c91a9fec4cbe681959ee3d63ad5470b533c0321c7ff4`  
		Last Modified: Fri, 21 Feb 2020 22:56:37 GMT  
		Size: 20.0 MB (20039487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ac24489f9fdaeb54802355163365f4f87bad194d7b24027388cfb4ca56df4fea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.4 MB (371436662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3c6a3cf0f1c255209b746986b92d3c5d7e2246952a1eb13c5dacbc7b321494`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:15:01 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefda6ea85dff94dd25f3c2b94cd56f646f91aa82300ab6b1a38c9682e8cd094`  
		Last Modified: Fri, 21 Feb 2020 23:42:39 GMT  
		Size: 20.9 MB (20946400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:fbb8763abcae1e23ebe2c4880f58a79a3c4782d5e82058d20d4ce3afb4e3c3e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:fc0fc6e27f939bbb8646cc906093cd28af2464673e1934e396365aa65c189eee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.2 MB (407205343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dad2b7cfd1c067a7254860051e5ba0c55032189a5019e3462beb2506a6de516`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:31:19 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8562cbcf9ab94f660f9ad756b3a323a24935a76950d87a81926201a133ae301f`  
		Last Modified: Sat, 22 Feb 2020 00:50:01 GMT  
		Size: 21.8 MB (21763751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:ec4e3aa73bf7b7f43ea433e778f5c36e1c190eb75dad41255c24dc82350afb6e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.7 MB (356714093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe58cf9ef47a1a053baa3228b26b3d29424475418e52557ca50877cbe73db89a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:29:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56cde4cae5f9a17754c91a9fec4cbe681959ee3d63ad5470b533c0321c7ff4`  
		Last Modified: Fri, 21 Feb 2020 22:56:37 GMT  
		Size: 20.0 MB (20039487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ac24489f9fdaeb54802355163365f4f87bad194d7b24027388cfb4ca56df4fea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.4 MB (371436662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3c6a3cf0f1c255209b746986b92d3c5d7e2246952a1eb13c5dacbc7b321494`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:15:01 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefda6ea85dff94dd25f3c2b94cd56f646f91aa82300ab6b1a38c9682e8cd094`  
		Last Modified: Fri, 21 Feb 2020 23:42:39 GMT  
		Size: 20.9 MB (20946400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:43d5ae157fc3c46f526b61b9c335c8eaedab78ff7ae20133b49891ffa61655bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2c075fb5be70e13dc96f087bc8eabe5cc64ee18a83982d780349c632d764476f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385441592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738ea393ac21a38436e6806c253439219c1b8c0161723043e806862701336b4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:3d718acd020242cba3e9a740e208ed095982711260c1e6a13693983cbfec4b45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336674606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57c3d3fb765b350d8332a08950d3d91a4f41e9e12043026591b4e851388f1e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fd760e573470a83df7e3d09b1e370fe5f39339eda7d4d53773184969536db6cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350490262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0ce788fbb9d15d7ba91bff960b7f189d2f043949d8b424aa0fe3c7d34fc9ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:43d5ae157fc3c46f526b61b9c335c8eaedab78ff7ae20133b49891ffa61655bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:2c075fb5be70e13dc96f087bc8eabe5cc64ee18a83982d780349c632d764476f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385441592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738ea393ac21a38436e6806c253439219c1b8c0161723043e806862701336b4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:30:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5206d27ca66c25c8a9841f68d38758b6a172e536d8607a78fa039c1e0d55a`  
		Last Modified: Sat, 22 Feb 2020 00:49:51 GMT  
		Size: 85.5 MB (85524380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:3d718acd020242cba3e9a740e208ed095982711260c1e6a13693983cbfec4b45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336674606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57c3d3fb765b350d8332a08950d3d91a4f41e9e12043026591b4e851388f1e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:29:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0cc25507c0c937150d1378f68e6116b97295bdf3a418fdc608ac5a790b6c87`  
		Last Modified: Fri, 21 Feb 2020 22:56:22 GMT  
		Size: 76.3 MB (76325822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fd760e573470a83df7e3d09b1e370fe5f39339eda7d4d53773184969536db6cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350490262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0ce788fbb9d15d7ba91bff960b7f189d2f043949d8b424aa0fe3c7d34fc9ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:14:08 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aa0fad8416cb5861b69e90ec6dbe97900dfe2997407d9ac13ce62e4bda216b`  
		Last Modified: Fri, 21 Feb 2020 23:42:19 GMT  
		Size: 77.8 MB (77819738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:ea30c1f3f2864d2ae6c24e5108e7932b289ff2c0ef88e223469cb8ba5f690044
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:aab52bbaeb4b9043eab8246e810bdbf34e5d2981a38873053c615cb37820bddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299917212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49a4e8508393aa9c539787c9b28a2f544cafa62eb31e6383c4cc9d18243f0e4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:57ccad6f8ce8efc61a0d234ec49967bcd361d4a0bb1c6641b8323436a20b2556
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260348784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c587ff89f3b2019e25b7d6cd5449acfb3e4b9f955bed6c5beeb48da3debdb3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f7c8e46026b0d00ddfe30cfca48d45a047312056c2856f1bfe233dfef5b9e03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272670524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d7134f7a6893f5c73fb8df47838548a2b20923e018a595e9b7eb0878ef88a6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:ea30c1f3f2864d2ae6c24e5108e7932b289ff2c0ef88e223469cb8ba5f690044
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:aab52bbaeb4b9043eab8246e810bdbf34e5d2981a38873053c615cb37820bddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299917212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49a4e8508393aa9c539787c9b28a2f544cafa62eb31e6383c4cc9d18243f0e4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:27:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:27:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:27:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:28:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:28:04 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:28:05 GMT
ENV ROS_DISTRO=kinetic
# Sat, 22 Feb 2020 00:28:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:29:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:29:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:29:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:29:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5a2e269056c8d304ca70dbb3df8cb043049caa1593349c0567d2b1800926d`  
		Last Modified: Sat, 22 Feb 2020 00:48:46 GMT  
		Size: 6.9 MB (6936216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8ea5750dd46479094654598598168f8632118dce36d0e00356d303689938e`  
		Last Modified: Sat, 22 Feb 2020 00:48:44 GMT  
		Size: 13.1 KB (13101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb110c86f88c42f992f9baba79944724cc65986e79d8626a415cb29b4421069`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d1c05d52300d66a89da8dd24a045a5d0cbc2a44f695ecb7da34c5299e383`  
		Last Modified: Sat, 22 Feb 2020 00:48:58 GMT  
		Size: 54.8 MB (54776668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09500c9f9db2638ab3a5fd6b7d51a74befe9cafde1c5702f00c10a3ef7d83e4e`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 425.0 KB (425030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbf4b9d57c61e0caef23140f26837706319c2b3370ebddc24a92b9434008fa5`  
		Last Modified: Sat, 22 Feb 2020 00:49:27 GMT  
		Size: 193.6 MB (193572507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e515d19e5c0b1ec72f4409b7a7c0ab7edaee124e3a6c39996a9d6d40897c2c6a`  
		Last Modified: Sat, 22 Feb 2020 00:48:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:57ccad6f8ce8efc61a0d234ec49967bcd361d4a0bb1c6641b8323436a20b2556
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260348784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c587ff89f3b2019e25b7d6cd5449acfb3e4b9f955bed6c5beeb48da3debdb3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:06:20 GMT
ADD file:7f245cd0bb5455d315f8d753720fab55e9ac41f68c7926b597663d3aeff3c8d4 in / 
# Fri, 21 Feb 2020 22:06:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:06:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:06:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:06:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:23:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:23:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:23:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:24:40 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:24:41 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:24:42 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 22:24:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:27:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:27:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:27:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:957d6015142d0d6fe598b45df39c8f36d0b86fe61fdb145603423c7d216e5f09`  
		Last Modified: Mon, 17 Feb 2020 15:45:30 GMT  
		Size: 38.9 MB (38890364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31e0e10e55fa8dad735b48b598b86efb29be81ae44906466ea04a2fd13c6c7`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42599b1b7e867902cc3b4a6cd7cd76c9148ff337a0bc7861131b6176648b45`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33654ecb4a4aa4b3b5b7f650b7aab38e3fe0d8d48d88c666f052f819016c3d55`  
		Last Modified: Fri, 21 Feb 2020 22:07:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67149689ed2c2bdb9efa3be9211d193b8028cc4784db0d6619a9390627191a5`  
		Last Modified: Fri, 21 Feb 2020 22:54:51 GMT  
		Size: 5.7 MB (5700209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95330f9d14ca033d17600bc8d8b11608f55728260b78bb4fd27004e672c4678`  
		Last Modified: Fri, 21 Feb 2020 22:54:49 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b787c40ff4d82dfe37e2e0a7011c7931ed7cb0007f131e5d046c99a784b91`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3da0282c816c36e5a182050d37ab4ff20cdd608c07e25dc928ddd8ddf18bc`  
		Last Modified: Fri, 21 Feb 2020 22:55:06 GMT  
		Size: 50.3 MB (50348544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1be963619c117704380dd2072975e251e911c6730b5b665535cdd33d12346`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 423.3 KB (423280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbfcd6ad198bc58083d92dde377c197dab923ea886b8d4ed0f04574e9262d2`  
		Last Modified: Fri, 21 Feb 2020 22:55:46 GMT  
		Size: 165.0 MB (164971335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9c520232387742ece66353864fde9c0eec372ea161e352369fd19d93be7957`  
		Last Modified: Fri, 21 Feb 2020 22:54:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f7c8e46026b0d00ddfe30cfca48d45a047312056c2856f1bfe233dfef5b9e03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272670524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d7134f7a6893f5c73fb8df47838548a2b20923e018a595e9b7eb0878ef88a6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:07:20 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:07:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:07:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:08:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:08:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:08:35 GMT
ENV ROS_DISTRO=kinetic
# Fri, 21 Feb 2020 23:08:53 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:11:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:12:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:12:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:12:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de89c3a73198e1dda189ac912dee05355cade0a829922bd13857425957eda71`  
		Last Modified: Fri, 21 Feb 2020 23:40:57 GMT  
		Size: 6.0 MB (5958466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9106380c300220f4bd02ff0b4648f292c64d767c8207b4e0e71534d4dd38961`  
		Last Modified: Fri, 21 Feb 2020 23:40:54 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208cdca92b9d0f49fd401ca56c0296caa856bf0b7b4f7d9af3ad99f4fa5ad32`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b569144b519d956769fd4db1b95a39e8afc6a4ca3e4a238d203404f4d4ceac1`  
		Last Modified: Fri, 21 Feb 2020 23:41:12 GMT  
		Size: 52.1 MB (52072482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a928563a652cdfddfb1e6dfdd83e83025d93c4b82eddf246fbb8687af9ed7a1c`  
		Last Modified: Fri, 21 Feb 2020 23:40:53 GMT  
		Size: 423.6 KB (423576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ab00cc30c740bb1569b4705e648bc226ba65f277626e6aa9cd6a2d43557f3`  
		Last Modified: Fri, 21 Feb 2020 23:41:45 GMT  
		Size: 174.3 MB (174260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f030f8f50f315846c4e32e83784be19ace559a52e3dd2cdf7926183de31bc00b`  
		Last Modified: Fri, 21 Feb 2020 23:40:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:ed8d141b40b9192b9228efe88a42afe8f89e75990792536298970ebadba1a1b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:678b09ba7e6fa38accde6f26cfb51d76974bcad6c6e763653a6c180cbc42456d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423970334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb1258d55457b86baedeef040cb2ac535cfb4487f6d119af1804f32f939b76e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm variant v7

```console
$ docker pull ros@sha256:658c44379df2914d04628905f2f7365ada08358eff27e059ad6dccc823af6860
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.8 MB (374835793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66b473118dc7c1f663a1f76fc9ce367c91018ba52a3fae6086924829d357f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8b67d3389e8331834721d1689e93120f1facf564ac77bfe93e97a16ead8c3b03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.6 MB (398563002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055731bcf8e0315c927077c84fa02361850c00f0e5b3e332a5ddadcc5bd2d5ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:ed8d141b40b9192b9228efe88a42afe8f89e75990792536298970ebadba1a1b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:678b09ba7e6fa38accde6f26cfb51d76974bcad6c6e763653a6c180cbc42456d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423970334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb1258d55457b86baedeef040cb2ac535cfb4487f6d119af1804f32f939b76e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:658c44379df2914d04628905f2f7365ada08358eff27e059ad6dccc823af6860
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.8 MB (374835793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66b473118dc7c1f663a1f76fc9ce367c91018ba52a3fae6086924829d357f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8b67d3389e8331834721d1689e93120f1facf564ac77bfe93e97a16ead8c3b03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.6 MB (398563002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055731bcf8e0315c927077c84fa02361850c00f0e5b3e332a5ddadcc5bd2d5ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:30b903e370bb98d8c4261768810b91564bb744020089022539b46d04fb545c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:ee37f858fbe94f4d627e04b0ebc261b6bbbd769bf06e43bcdbeb077ce74afa34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **774.1 MB (774125607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9100b0f32f3fcfcd06b92df0cd62bbe98ace483b692f600cd4123512e5143139`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:44:09 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd10d1127094a562b0bf73b2b6c87770353873d3d4aaa58b0a2565bc85a424`  
		Last Modified: Sat, 22 Feb 2020 00:54:03 GMT  
		Size: 350.2 MB (350155273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:6b45cef7c0bbe7a6ab094630ca18ca5ae58aa14c129ec11116915a43d9cb48a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **675.0 MB (674959937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5faa98fd9c4e0fa322308145753bf037041e14f7246f43c294759461c840db0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:46:25 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087e416e86852c6c4664b629e772f567e4932686f17d4dca1078f19af27f7a60`  
		Last Modified: Fri, 21 Feb 2020 23:02:46 GMT  
		Size: 300.1 MB (300124144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7aa62ce8d2146296c9286a0ffe79dc09ef73c559cec50c6dbd37120c16374f0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **731.4 MB (731395990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:140bce82fafff8f2a00e7927d38071b816fc60d38552d1be9dfa8ce4fd8e29b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:31:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f800e8ca697cbaf7c47848df67142291f042b973f3d453355990917ce3d772ef`  
		Last Modified: Fri, 21 Feb 2020 23:48:01 GMT  
		Size: 332.8 MB (332832988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:30b903e370bb98d8c4261768810b91564bb744020089022539b46d04fb545c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:ee37f858fbe94f4d627e04b0ebc261b6bbbd769bf06e43bcdbeb077ce74afa34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **774.1 MB (774125607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9100b0f32f3fcfcd06b92df0cd62bbe98ace483b692f600cd4123512e5143139`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:44:09 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd10d1127094a562b0bf73b2b6c87770353873d3d4aaa58b0a2565bc85a424`  
		Last Modified: Sat, 22 Feb 2020 00:54:03 GMT  
		Size: 350.2 MB (350155273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:6b45cef7c0bbe7a6ab094630ca18ca5ae58aa14c129ec11116915a43d9cb48a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **675.0 MB (674959937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5faa98fd9c4e0fa322308145753bf037041e14f7246f43c294759461c840db0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:46:25 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087e416e86852c6c4664b629e772f567e4932686f17d4dca1078f19af27f7a60`  
		Last Modified: Fri, 21 Feb 2020 23:02:46 GMT  
		Size: 300.1 MB (300124144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7aa62ce8d2146296c9286a0ffe79dc09ef73c559cec50c6dbd37120c16374f0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **731.4 MB (731395990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:140bce82fafff8f2a00e7927d38071b816fc60d38552d1be9dfa8ce4fd8e29b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:31:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f800e8ca697cbaf7c47848df67142291f042b973f3d453355990917ce3d772ef`  
		Last Modified: Fri, 21 Feb 2020 23:48:01 GMT  
		Size: 332.8 MB (332832988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:be6d783ff0e24eac1aea7f92676741dfdb21a922553ef472c67c4e33f5145769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:61580feb9ab028dd5499faf30287406c087d3a1ba4b7bd06283b1578ce49a8bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **876.2 MB (876206669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ac3ef7ac1e89d9abb3bb3ab21353226bac9d190adcdf80781ae6033220a7c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:49:37 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:49:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 01 Feb 2020 18:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 01 Feb 2020 18:50:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:50:37 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 18:50:38 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Feb 2020 00:04:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Feb 2020 00:05:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Feb 2020 00:06:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 06 Feb 2020 00:06:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Feb 2020 00:06:14 GMT
CMD ["bash"]
# Thu, 06 Feb 2020 00:06:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:09:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905ca7a93e1f1f1e5a3c9d5dacdf39395a357b216f42962d54cb9f2f2779419`  
		Last Modified: Sat, 01 Feb 2020 18:59:03 GMT  
		Size: 10.5 MB (10476666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d9067426f73e53072c040a66d4e587fa9badca3da3aed990b6ef8afe8385b`  
		Last Modified: Sat, 01 Feb 2020 18:59:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47253481cad39c6f079e90a602a37b6638204f66869e48320e2d414b8ec82be5`  
		Last Modified: Sat, 01 Feb 2020 18:59:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822fec1fbb983df499d36a4c4325090bc1538e03ea008262104c269ccf6d6dc4`  
		Last Modified: Sat, 01 Feb 2020 18:59:18 GMT  
		Size: 64.8 MB (64771303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16863f4abfb019c6e8a8fea1c6e62b6143066c7f5e93a79efe3e9b651ebc248`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 416.3 KB (416299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16c2d9ace030f8cf7130554cca720123d8d98ac042030446e8e63d2fed7575`  
		Last Modified: Thu, 06 Feb 2020 00:24:16 GMT  
		Size: 270.4 MB (270396052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dc5fb275b853031a6119ad6970232236aa67ec1091eb754ef605ddcdb0ec0`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989e70d294fe3d20b5496caf95ff8bbbd3a87f2767957b524094176593b4b0`  
		Last Modified: Thu, 06 Feb 2020 00:25:02 GMT  
		Size: 108.5 MB (108474848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86431303289738ae5c285bf6f5ca2b267cf554a458dc975cf0e15c51a30a607`  
		Last Modified: Thu, 06 Feb 2020 00:28:11 GMT  
		Size: 376.3 MB (376289025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:899d15806249b4eae85cf03103269c1704ca6433cec058a117800eb8c47f7a1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **794.1 MB (794089435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c39cf5d681773c4314ecebe009be49051a9a313dfd42997c82c4e968fd810cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:31:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:31:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Feb 2020 14:31:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Feb 2020 14:33:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:33:23 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:33:24 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Feb 2020 14:33:25 GMT
ENV ROS_DISTRO=melodic
# Wed, 26 Feb 2020 14:33:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Feb 2020 14:36:54 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:37:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Feb 2020 14:37:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Feb 2020 14:37:12 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:45:34 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec93ccfa7a93f6e8e92bfb6a4612d88201a991de0eeccbf0f0bf911e494b010`  
		Last Modified: Wed, 26 Feb 2020 14:46:38 GMT  
		Size: 9.8 MB (9774844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d47cc5c856874753256905adae1cafc7bbe555293057734a15adff043ad552`  
		Last Modified: Wed, 26 Feb 2020 14:46:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8904c2c29a9d325e34d20fc23a9bf0424e4011a33a408e44efc9d3a7afd762`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd405032f54a80c542f1c495a333e79235726b6bc13a929b1cd5b8c1857cf4da`  
		Last Modified: Wed, 26 Feb 2020 14:47:00 GMT  
		Size: 62.1 MB (62091345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22cef13f13ce297cd764e86e8e695631eb4f9bd35437f30cb2fb4121836e4f`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 426.5 KB (426457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c556607af67c09197a3819a5d4186a8a16161d13034880bcfa9896a95453d8ee`  
		Last Modified: Wed, 26 Feb 2020 14:47:46 GMT  
		Size: 224.6 MB (224601602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61457eaec54891acb526a2385adff233378c15c155753857cab7397dfce078c`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d522db6c8689265e2a824a336e54ef5e1d066934054d93dd8a56e3fb7098a9`  
		Last Modified: Wed, 26 Feb 2020 14:48:16 GMT  
		Size: 103.0 MB (102962444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bf274cb17c6582671fe3a999cc0756fe487424f5b0d308cb20f1c6323ea94a`  
		Last Modified: Wed, 26 Feb 2020 14:50:09 GMT  
		Size: 351.1 MB (351072776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:7e8616c8f05646725b11b03f0e51e9ad2747b4c89d5eeb4c683831e846cd208b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:7d5afca6f9450e094cedbbaf8eaf49abdd391ef804d472b2b8ef70c0d7802d49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **438.8 MB (438764316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952a207fbe035ce91f9b1d5ef8bf390fd8cf86cabd787a3b94fc6d108a576ee8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:39:04 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bae4873054521c47613e51396d9e7eb900ef9ca80743109f2bcfbb451e5fb89`  
		Last Modified: Sat, 22 Feb 2020 00:52:46 GMT  
		Size: 14.8 MB (14793982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:4bacf9df86627032d53aa701e73c267c89324149e09b98256437a640ccfa3de3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.6 MB (388568947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c838898dd37f90f0440752a860e6545cb294ecc8871b4431b4a582dfbc9f12e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:41:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a8b01a0e8426fe4e63d7c570c0df68bd803e5ea661ad8dd447d11d16a6a39`  
		Last Modified: Fri, 21 Feb 2020 23:01:05 GMT  
		Size: 13.7 MB (13733154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f82846a02a6bfb97138f10e278bd449d391db57111783b796d3a83dc4f3882c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.8 MB (412815182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f541d0920aa569ab14075e113ca6a9c07a2a103b7f3a7e5151fdc5461f33ecf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806406b37792eca9412d29b15554f098be3ddadc76d3c0f56b4120d25cd7c2e2`  
		Last Modified: Fri, 21 Feb 2020 23:46:14 GMT  
		Size: 14.3 MB (14252180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:7e8616c8f05646725b11b03f0e51e9ad2747b4c89d5eeb4c683831e846cd208b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:7d5afca6f9450e094cedbbaf8eaf49abdd391ef804d472b2b8ef70c0d7802d49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **438.8 MB (438764316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952a207fbe035ce91f9b1d5ef8bf390fd8cf86cabd787a3b94fc6d108a576ee8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:39:04 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bae4873054521c47613e51396d9e7eb900ef9ca80743109f2bcfbb451e5fb89`  
		Last Modified: Sat, 22 Feb 2020 00:52:46 GMT  
		Size: 14.8 MB (14793982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:4bacf9df86627032d53aa701e73c267c89324149e09b98256437a640ccfa3de3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.6 MB (388568947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c838898dd37f90f0440752a860e6545cb294ecc8871b4431b4a582dfbc9f12e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:41:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a8b01a0e8426fe4e63d7c570c0df68bd803e5ea661ad8dd447d11d16a6a39`  
		Last Modified: Fri, 21 Feb 2020 23:01:05 GMT  
		Size: 13.7 MB (13733154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f82846a02a6bfb97138f10e278bd449d391db57111783b796d3a83dc4f3882c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.8 MB (412815182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f541d0920aa569ab14075e113ca6a9c07a2a103b7f3a7e5151fdc5461f33ecf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806406b37792eca9412d29b15554f098be3ddadc76d3c0f56b4120d25cd7c2e2`  
		Last Modified: Fri, 21 Feb 2020 23:46:14 GMT  
		Size: 14.3 MB (14252180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:2ec4f379e4a30da5cd2301fa5fe5376ca9a178a1af4427511bfcce8a43f8d8c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:5309d6bc6a1e371c38a7ea720f3e4c7eab363b4283b3d0e86e347ce590d41a5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **518.8 MB (518801512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef452033f1a3eb7a9163240087cae6a15063200e1f9bc0e3250c1f892528ef7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:49:37 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:49:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 01 Feb 2020 18:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 01 Feb 2020 18:50:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:50:37 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 18:50:38 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Feb 2020 00:04:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Feb 2020 00:05:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Feb 2020 00:06:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 06 Feb 2020 00:06:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Feb 2020 00:06:14 GMT
CMD ["bash"]
# Thu, 06 Feb 2020 00:06:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:07:27 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905ca7a93e1f1f1e5a3c9d5dacdf39395a357b216f42962d54cb9f2f2779419`  
		Last Modified: Sat, 01 Feb 2020 18:59:03 GMT  
		Size: 10.5 MB (10476666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d9067426f73e53072c040a66d4e587fa9badca3da3aed990b6ef8afe8385b`  
		Last Modified: Sat, 01 Feb 2020 18:59:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47253481cad39c6f079e90a602a37b6638204f66869e48320e2d414b8ec82be5`  
		Last Modified: Sat, 01 Feb 2020 18:59:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822fec1fbb983df499d36a4c4325090bc1538e03ea008262104c269ccf6d6dc4`  
		Last Modified: Sat, 01 Feb 2020 18:59:18 GMT  
		Size: 64.8 MB (64771303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16863f4abfb019c6e8a8fea1c6e62b6143066c7f5e93a79efe3e9b651ebc248`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 416.3 KB (416299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16c2d9ace030f8cf7130554cca720123d8d98ac042030446e8e63d2fed7575`  
		Last Modified: Thu, 06 Feb 2020 00:24:16 GMT  
		Size: 270.4 MB (270396052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dc5fb275b853031a6119ad6970232236aa67ec1091eb754ef605ddcdb0ec0`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989e70d294fe3d20b5496caf95ff8bbbd3a87f2767957b524094176593b4b0`  
		Last Modified: Thu, 06 Feb 2020 00:25:02 GMT  
		Size: 108.5 MB (108474848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48acfe3e6448d771edf6c928458b2e5cbe5dae5edc4e219005163fa45b161a6c`  
		Last Modified: Thu, 06 Feb 2020 00:25:23 GMT  
		Size: 18.9 MB (18883868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d00a55197391be2fdbbd9d4a6515f99c52a283696b185261ece98c23a56d540d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.2 MB (461244123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4396a382cadac7dfbc1d1d585285d1c90f6446a4a29b9923f65be8bc85904eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:31:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:31:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Feb 2020 14:31:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Feb 2020 14:33:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:33:23 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:33:24 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Feb 2020 14:33:25 GMT
ENV ROS_DISTRO=melodic
# Wed, 26 Feb 2020 14:33:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Feb 2020 14:36:54 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:37:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Feb 2020 14:37:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Feb 2020 14:37:12 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:39:53 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec93ccfa7a93f6e8e92bfb6a4612d88201a991de0eeccbf0f0bf911e494b010`  
		Last Modified: Wed, 26 Feb 2020 14:46:38 GMT  
		Size: 9.8 MB (9774844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d47cc5c856874753256905adae1cafc7bbe555293057734a15adff043ad552`  
		Last Modified: Wed, 26 Feb 2020 14:46:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8904c2c29a9d325e34d20fc23a9bf0424e4011a33a408e44efc9d3a7afd762`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd405032f54a80c542f1c495a333e79235726b6bc13a929b1cd5b8c1857cf4da`  
		Last Modified: Wed, 26 Feb 2020 14:47:00 GMT  
		Size: 62.1 MB (62091345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22cef13f13ce297cd764e86e8e695631eb4f9bd35437f30cb2fb4121836e4f`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 426.5 KB (426457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c556607af67c09197a3819a5d4186a8a16161d13034880bcfa9896a95453d8ee`  
		Last Modified: Wed, 26 Feb 2020 14:47:46 GMT  
		Size: 224.6 MB (224601602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61457eaec54891acb526a2385adff233378c15c155753857cab7397dfce078c`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d522db6c8689265e2a824a336e54ef5e1d066934054d93dd8a56e3fb7098a9`  
		Last Modified: Wed, 26 Feb 2020 14:48:16 GMT  
		Size: 103.0 MB (102962444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35402575745d94cb092a62316cfe5bc66cc1a9fb9bb7247231e3e56b1c50d663`  
		Last Modified: Wed, 26 Feb 2020 14:48:27 GMT  
		Size: 18.2 MB (18227464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:ed8d141b40b9192b9228efe88a42afe8f89e75990792536298970ebadba1a1b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:678b09ba7e6fa38accde6f26cfb51d76974bcad6c6e763653a6c180cbc42456d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423970334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb1258d55457b86baedeef040cb2ac535cfb4487f6d119af1804f32f939b76e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:658c44379df2914d04628905f2f7365ada08358eff27e059ad6dccc823af6860
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.8 MB (374835793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66b473118dc7c1f663a1f76fc9ce367c91018ba52a3fae6086924829d357f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8b67d3389e8331834721d1689e93120f1facf564ac77bfe93e97a16ead8c3b03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.6 MB (398563002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055731bcf8e0315c927077c84fa02361850c00f0e5b3e332a5ddadcc5bd2d5ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:ed8d141b40b9192b9228efe88a42afe8f89e75990792536298970ebadba1a1b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:678b09ba7e6fa38accde6f26cfb51d76974bcad6c6e763653a6c180cbc42456d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423970334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb1258d55457b86baedeef040cb2ac535cfb4487f6d119af1804f32f939b76e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
# Sat, 22 Feb 2020 00:38:31 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18db02e9f6fd85a4b089996b8dca7a0248ba13c3c10f5221d49d8184b8a556cf`  
		Last Modified: Sat, 22 Feb 2020 00:52:35 GMT  
		Size: 72.9 MB (72918450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:658c44379df2914d04628905f2f7365ada08358eff27e059ad6dccc823af6860
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.8 MB (374835793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66b473118dc7c1f663a1f76fc9ce367c91018ba52a3fae6086924829d357f4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 22:41:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2216ed99d366635379b49f2ead9115ece271f64298c83f24f5153b303c34af82`  
		Last Modified: Fri, 21 Feb 2020 23:00:05 GMT  
		Size: 62.9 MB (62874295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8b67d3389e8331834721d1689e93120f1facf564ac77bfe93e97a16ead8c3b03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.6 MB (398563002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055731bcf8e0315c927077c84fa02361850c00f0e5b3e332a5ddadcc5bd2d5ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
# Fri, 21 Feb 2020 23:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeafb8da4283d3a220685745dd74780389e4f9f82cfd1afee235b59c13bd57e`  
		Last Modified: Fri, 21 Feb 2020 23:45:59 GMT  
		Size: 65.6 MB (65554933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:d05635c7520e2ccbec122911ae69da341b5d457e1b9188a1b0ebbc7c6ab80e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:dae34e8594a8c322ac2dc7403a084bf5e4f4d729f0db41d65697c534767b3ae4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.9 MB (499917644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04da5b50c44b2e66788ca85088abc106e99db345e77a56b714f6ec0e8f68bcb7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:49:37 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:49:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 01 Feb 2020 18:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 01 Feb 2020 18:50:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:50:37 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 18:50:38 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Feb 2020 00:04:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Feb 2020 00:05:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Feb 2020 00:06:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 06 Feb 2020 00:06:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Feb 2020 00:06:14 GMT
CMD ["bash"]
# Thu, 06 Feb 2020 00:06:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905ca7a93e1f1f1e5a3c9d5dacdf39395a357b216f42962d54cb9f2f2779419`  
		Last Modified: Sat, 01 Feb 2020 18:59:03 GMT  
		Size: 10.5 MB (10476666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d9067426f73e53072c040a66d4e587fa9badca3da3aed990b6ef8afe8385b`  
		Last Modified: Sat, 01 Feb 2020 18:59:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47253481cad39c6f079e90a602a37b6638204f66869e48320e2d414b8ec82be5`  
		Last Modified: Sat, 01 Feb 2020 18:59:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822fec1fbb983df499d36a4c4325090bc1538e03ea008262104c269ccf6d6dc4`  
		Last Modified: Sat, 01 Feb 2020 18:59:18 GMT  
		Size: 64.8 MB (64771303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16863f4abfb019c6e8a8fea1c6e62b6143066c7f5e93a79efe3e9b651ebc248`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 416.3 KB (416299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16c2d9ace030f8cf7130554cca720123d8d98ac042030446e8e63d2fed7575`  
		Last Modified: Thu, 06 Feb 2020 00:24:16 GMT  
		Size: 270.4 MB (270396052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dc5fb275b853031a6119ad6970232236aa67ec1091eb754ef605ddcdb0ec0`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989e70d294fe3d20b5496caf95ff8bbbd3a87f2767957b524094176593b4b0`  
		Last Modified: Thu, 06 Feb 2020 00:25:02 GMT  
		Size: 108.5 MB (108474848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2faade4fe6adba2f9cca34336cbb2d155e8fe412c5153563cd9a55cea7147697
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.0 MB (443016659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9445d40e3b8f06c7cb6d2de0edbadeba82e5a7da4755733ec346c9dfa9d632`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:31:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:31:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Feb 2020 14:31:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Feb 2020 14:33:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:33:23 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:33:24 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Feb 2020 14:33:25 GMT
ENV ROS_DISTRO=melodic
# Wed, 26 Feb 2020 14:33:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Feb 2020 14:36:54 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:37:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Feb 2020 14:37:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Feb 2020 14:37:12 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec93ccfa7a93f6e8e92bfb6a4612d88201a991de0eeccbf0f0bf911e494b010`  
		Last Modified: Wed, 26 Feb 2020 14:46:38 GMT  
		Size: 9.8 MB (9774844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d47cc5c856874753256905adae1cafc7bbe555293057734a15adff043ad552`  
		Last Modified: Wed, 26 Feb 2020 14:46:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8904c2c29a9d325e34d20fc23a9bf0424e4011a33a408e44efc9d3a7afd762`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd405032f54a80c542f1c495a333e79235726b6bc13a929b1cd5b8c1857cf4da`  
		Last Modified: Wed, 26 Feb 2020 14:47:00 GMT  
		Size: 62.1 MB (62091345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22cef13f13ce297cd764e86e8e695631eb4f9bd35437f30cb2fb4121836e4f`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 426.5 KB (426457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c556607af67c09197a3819a5d4186a8a16161d13034880bcfa9896a95453d8ee`  
		Last Modified: Wed, 26 Feb 2020 14:47:46 GMT  
		Size: 224.6 MB (224601602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61457eaec54891acb526a2385adff233378c15c155753857cab7397dfce078c`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d522db6c8689265e2a824a336e54ef5e1d066934054d93dd8a56e3fb7098a9`  
		Last Modified: Wed, 26 Feb 2020 14:48:16 GMT  
		Size: 103.0 MB (102962444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:985f1a7bf617d04e7f0d967e13ac92b4f141010a2fd16a5a2de3fe8e660d8540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:80e4c5452234f6564abcfa939c240eae37b66d4cd7375ddc6c0b3acf50c4d443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.1 MB (351051884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86441d9c8b9f0f5e0961f8cd46d28ef36c1799d81c5ae1f0cd142703ec45d733`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:2f5acb331f70cfc029c29da935095c23c2b2b1269ecabf41e6b3c993a7ad97a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.0 MB (311961498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a28f440224c1c4ff3a04e6ca7a415f189bb86a9e4266b3a7eab69a652cca5b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1249cd82f1f21451b88275fc47e0f5d2387a1e3c46a7f441b2bc3a59f1b9496
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (333008069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c741628226f0205748a78d395558dd7c3892de86f1596c8f4b2c8be8f4cbd4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:985f1a7bf617d04e7f0d967e13ac92b4f141010a2fd16a5a2de3fe8e660d8540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:80e4c5452234f6564abcfa939c240eae37b66d4cd7375ddc6c0b3acf50c4d443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.1 MB (351051884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86441d9c8b9f0f5e0961f8cd46d28ef36c1799d81c5ae1f0cd142703ec45d733`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:33:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:49 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:34:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 22 Feb 2020 00:34:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 22 Feb 2020 00:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:35:36 GMT
ENV LANG=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV LC_ALL=C.UTF-8
# Sat, 22 Feb 2020 00:35:37 GMT
ENV ROS_DISTRO=melodic
# Sat, 22 Feb 2020 00:35:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 22 Feb 2020 00:37:26 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:37:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 22 Feb 2020 00:37:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 22 Feb 2020 00:37:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe4c16cf9b0d96d5ca63260c28e39ec2082af1f69bdc406d460e68fd3378f0`  
		Last Modified: Fri, 21 Feb 2020 23:47:45 GMT  
		Size: 838.2 KB (838151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241889f00501354e18c8698434ace91d2276551d63ef1ed65afe92a82fec0666`  
		Last Modified: Sat, 22 Feb 2020 00:51:24 GMT  
		Size: 6.8 MB (6779039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a766c4ee10313a4d3b338dede3cdd0bc0d3ff4e89588c57ca4a5f8655f5e769`  
		Last Modified: Sat, 22 Feb 2020 00:51:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90f780b8a93b1edcce4a3249f651bb6e9df0db35030bd7d668f882eff5788b`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a1de819665075cc1704aa873ab98fb88f4e2b53e5bbaaafb977b6704553ef`  
		Last Modified: Sat, 22 Feb 2020 00:51:36 GMT  
		Size: 55.1 MB (55077154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d9e96c6ba0ae8d2d631c499d06f6c563af0555d36dbcb63456e542793f3cf`  
		Last Modified: Sat, 22 Feb 2020 00:51:21 GMT  
		Size: 425.0 KB (425031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd295e4dce379c10846839ff06b6c244c41d239c398e4c940cc0a735b27c86`  
		Last Modified: Sat, 22 Feb 2020 00:52:13 GMT  
		Size: 261.2 MB (261202196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6a7c9d722aeb05e8594dda3f5559840987dfeadccccd98d44ce6e6e32e9e2b`  
		Last Modified: Sat, 22 Feb 2020 00:51:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:2f5acb331f70cfc029c29da935095c23c2b2b1269ecabf41e6b3c993a7ad97a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.0 MB (311961498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a28f440224c1c4ff3a04e6ca7a415f189bb86a9e4266b3a7eab69a652cca5b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:04:48 GMT
ADD file:548fc3249b705bf3e94efcc50c1c9141e03d1ce51edfc194a84bd631d1a7b6d4 in / 
# Fri, 21 Feb 2020 22:04:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:02 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:34:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:35:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 22:35:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:36:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 22:36:29 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 22:36:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 22:39:21 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 22:39:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 22:39:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9b5ae93466ea2cca8f47e7e02dc1907faaaae6ed617360e47259eb4cac4d0a7`  
		Last Modified: Fri, 21 Feb 2020 22:06:53 GMT  
		Size: 22.3 MB (22275658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8983199234a3f5beecbe2be6e21b4a49e67dd5726e7080e999c6f2cea91bc2`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 35.5 KB (35470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f87f706a4e3e6b5f3d9fabd021b46b875dc9058e26d31877057069115333`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196ba84f492bbca6bb4979ae6e8d2d3a952559cdf3dfd11e99c3a4c11aa0891`  
		Last Modified: Fri, 21 Feb 2020 22:06:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94681626ece376a18f3e47c882222f1de6ea03203910197f3121573b1854cf`  
		Last Modified: Fri, 21 Feb 2020 22:58:20 GMT  
		Size: 838.0 KB (838036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53015c31a2edd4faf338cbdbc2c917ec78f2be36e6010454d2a7d99e0f23b8bb`  
		Last Modified: Fri, 21 Feb 2020 22:58:21 GMT  
		Size: 5.6 MB (5629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3883ec0f148a13093bbc85ad6c3f1123375f8fbe936102c4a22ad4d408ed`  
		Last Modified: Fri, 21 Feb 2020 22:58:18 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc625ea4f04535f4ae43a546e47f26edbde5e63572e7ae7f4f70b95ee758c5`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86753701ddf5abb8e747e3d298a95b70cd2068318684ef8b7dd0e4ddb848be2f`  
		Last Modified: Fri, 21 Feb 2020 22:58:36 GMT  
		Size: 50.1 MB (50113606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0449c8520098d9eccd396e25ab7caaf2e6bb7b7a539086efc6aae3c5ef4df`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 423.3 KB (423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3201f5a81f4f64027f1c0f10a924e677970877eba1a8d73b67cbf3fcfdf5628`  
		Last Modified: Fri, 21 Feb 2020 22:59:33 GMT  
		Size: 232.6 MB (232642898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4b0b28b3a94eaa46408e6fb6cf7d202c7c24c794a10a5a029086506baefb`  
		Last Modified: Fri, 21 Feb 2020 22:58:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1249cd82f1f21451b88275fc47e0f5d2387a1e3c46a7f441b2bc3a59f1b9496
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (333008069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c741628226f0205748a78d395558dd7c3892de86f1596c8f4b2c8be8f4cbd4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:19:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:43 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:19:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 21 Feb 2020 23:19:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 21 Feb 2020 23:20:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:20:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Feb 2020 23:20:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 21 Feb 2020 23:20:58 GMT
ENV ROS_DISTRO=melodic
# Fri, 21 Feb 2020 23:21:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 21 Feb 2020 23:24:19 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:24:32 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 21 Feb 2020 23:24:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9245e73b2caf8b938074b23c3c20fbcce64fd1928003222258b8814ca4d7659`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 838.1 KB (838054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9a1a1ddbaf11b914cf9d5f5f8a0e0f57e6f73c5a61b54ff2c353e9d7f7395`  
		Last Modified: Fri, 21 Feb 2020 23:44:30 GMT  
		Size: 6.1 MB (6096311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86484c6fdf800f448e5e83532268dc42a783100c7d6dc0b849f984c506fee84d`  
		Last Modified: Fri, 21 Feb 2020 23:44:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0434ef313cf02aa5fc79ee52d391ad5e396911673ea10d7ef8707adec8bd0c3e`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde59e075d0822c568c764e1af8e141ab48c594aa40aec2013196c762ed0b30`  
		Last Modified: Fri, 21 Feb 2020 23:44:43 GMT  
		Size: 52.9 MB (52924621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8139fba839857061131efa91eedc0135b114953a7507b2d226d1b02c027717b`  
		Last Modified: Fri, 21 Feb 2020 23:44:26 GMT  
		Size: 423.6 KB (423564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daced03c7e3e0dfd7303a7d8781a6771d94f90bc7549890e543221cee2dc73bb`  
		Last Modified: Fri, 21 Feb 2020 23:45:32 GMT  
		Size: 249.0 MB (248966300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb899009cc0ab7c7b4bb6f6da04dff60397816441ed8c7213e4959a06a479f5`  
		Last Modified: Fri, 21 Feb 2020 23:44:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:667fb562c2c98b41fe0c0f333b13efb2e791607647a885c400312970a60842ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:9089d6cbb3e59377cb8ceb41bb0446a2c9f412f82e95115260dbafe335f17e20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391442796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f0a4743794ddf3c85797ea07541eaa9ef1bd05bd28ec47ec9e015b7999c0f1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:49:37 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:49:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 01 Feb 2020 18:49:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 01 Feb 2020 18:50:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:50:37 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 18:50:38 GMT
ENV LC_ALL=C.UTF-8
# Thu, 06 Feb 2020 00:04:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 06 Feb 2020 00:05:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 06 Feb 2020 00:06:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Feb 2020 00:06:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 06 Feb 2020 00:06:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 06 Feb 2020 00:06:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905ca7a93e1f1f1e5a3c9d5dacdf39395a357b216f42962d54cb9f2f2779419`  
		Last Modified: Sat, 01 Feb 2020 18:59:03 GMT  
		Size: 10.5 MB (10476666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d9067426f73e53072c040a66d4e587fa9badca3da3aed990b6ef8afe8385b`  
		Last Modified: Sat, 01 Feb 2020 18:59:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47253481cad39c6f079e90a602a37b6638204f66869e48320e2d414b8ec82be5`  
		Last Modified: Sat, 01 Feb 2020 18:59:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822fec1fbb983df499d36a4c4325090bc1538e03ea008262104c269ccf6d6dc4`  
		Last Modified: Sat, 01 Feb 2020 18:59:18 GMT  
		Size: 64.8 MB (64771303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16863f4abfb019c6e8a8fea1c6e62b6143066c7f5e93a79efe3e9b651ebc248`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 416.3 KB (416299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16c2d9ace030f8cf7130554cca720123d8d98ac042030446e8e63d2fed7575`  
		Last Modified: Thu, 06 Feb 2020 00:24:16 GMT  
		Size: 270.4 MB (270396052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dc5fb275b853031a6119ad6970232236aa67ec1091eb754ef605ddcdb0ec0`  
		Last Modified: Thu, 06 Feb 2020 00:22:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bccee9c4d9a13ea6bdbcc2e78cfd4418ea55e280eb64eda7830cc015ef3f89a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340054215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d2ec2d310b6a937ce2abd3513c573baf887dbf29253d85d79db64f7cde2f927`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:31:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:31:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Feb 2020 14:31:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Feb 2020 14:33:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:33:23 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:33:24 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Feb 2020 14:33:25 GMT
ENV ROS_DISTRO=melodic
# Wed, 26 Feb 2020 14:33:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Feb 2020 14:36:54 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:37:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Feb 2020 14:37:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Feb 2020 14:37:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec93ccfa7a93f6e8e92bfb6a4612d88201a991de0eeccbf0f0bf911e494b010`  
		Last Modified: Wed, 26 Feb 2020 14:46:38 GMT  
		Size: 9.8 MB (9774844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d47cc5c856874753256905adae1cafc7bbe555293057734a15adff043ad552`  
		Last Modified: Wed, 26 Feb 2020 14:46:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8904c2c29a9d325e34d20fc23a9bf0424e4011a33a408e44efc9d3a7afd762`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd405032f54a80c542f1c495a333e79235726b6bc13a929b1cd5b8c1857cf4da`  
		Last Modified: Wed, 26 Feb 2020 14:47:00 GMT  
		Size: 62.1 MB (62091345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22cef13f13ce297cd764e86e8e695631eb4f9bd35437f30cb2fb4121836e4f`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 426.5 KB (426457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c556607af67c09197a3819a5d4186a8a16161d13034880bcfa9896a95453d8ee`  
		Last Modified: Wed, 26 Feb 2020 14:47:46 GMT  
		Size: 224.6 MB (224601602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61457eaec54891acb526a2385adff233378c15c155753857cab7397dfce078c`  
		Last Modified: Wed, 26 Feb 2020 14:46:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
