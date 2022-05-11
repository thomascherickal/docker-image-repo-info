## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:6d370be3c70b2498fdbcf676b3a0db1d83c045993942d530c5a153d7d8299b39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:8de1b92b0e71a90fa026b120c9151cbc09d14cc2596e24f9abe6108e85577c0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.8 MB (484800165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85faa48836173c820ff0176e00c368331e4cb1964d933a05b160ab32a342238f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:08:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:08:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 May 2022 16:08:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 May 2022 16:08:27 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 16:08:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 May 2022 16:08:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 May 2022 16:09:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:09:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 11 May 2022 16:09:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 May 2022 16:09:28 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:09:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:10:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 May 2022 16:10:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:10:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7806f53f52d18737a208f3d99a352a6a818aca1737f3036e6cdd2558cb8c2878`  
		Last Modified: Wed, 11 May 2022 16:14:00 GMT  
		Size: 10.9 MB (10892016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abfabd810e159ce51f93f3439c49a3eb065c9cabccfd2ff19aa1f2e973cbc8f`  
		Last Modified: Wed, 11 May 2022 16:13:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df902248ee6ae3eff3eaec0243df161bf028617ee930cbf1b96e389230c0bb`  
		Last Modified: Wed, 11 May 2022 16:13:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fc9931a4cac56fa18fbdd7e81f03ca32b58b2630f364331ba224eec67fe7e1`  
		Last Modified: Wed, 11 May 2022 16:14:32 GMT  
		Size: 239.2 MB (239167058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef75ff8b7b329e7b59d3dd6d4bd0c62f9f83d1b406614acf18d686120abf3af2`  
		Last Modified: Wed, 11 May 2022 16:13:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9e1921a71fbfd8587eff972b0ca2ab1c88fac6b724fca05ef782fee13e349`  
		Last Modified: Wed, 11 May 2022 16:14:52 GMT  
		Size: 86.6 MB (86566357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d405c1b5e75348658978f1bf086d70164a6876f429f9dee962256c0c66b6bde`  
		Last Modified: Wed, 11 May 2022 16:14:40 GMT  
		Size: 311.5 KB (311492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88dce7ef6e2637a6141f769e7c9b78665bca3886f20a940d6eb428b23e5e81f`  
		Last Modified: Wed, 11 May 2022 16:14:50 GMT  
		Size: 76.0 MB (75976162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c3ac2b9c62bac573a37a669d6fed5dba4d6ee0aa1500aeee5a8150292b1c77`  
		Last Modified: Wed, 11 May 2022 16:15:02 GMT  
		Size: 21.4 MB (21446704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4b2c2cd07bb9c407c755bdf22e6ba6730be5a086db58233bb4fa706f2a9a3455
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423930213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25196c0b0c9f21abe17e5a42d6e2cff80ebc4484358b15ec45a6b4f9dcb993aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:06:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:06:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 11 May 2022 12:06:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 11 May 2022 12:06:29 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 12:06:30 GMT
ENV LC_ALL=C.UTF-8
# Wed, 11 May 2022 12:06:31 GMT
ENV ROS_DISTRO=noetic
# Wed, 11 May 2022 12:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:07:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 11 May 2022 12:07:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 11 May 2022 12:07:53 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:08:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:08:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 11 May 2022 12:08:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b8f001a81871a79288c49f8da44f6046802fe74b7657025c69cff9763f4e8`  
		Last Modified: Wed, 11 May 2022 12:14:33 GMT  
		Size: 10.7 MB (10688182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c15bb481e3ba1f71bde43e29ea4709894051d2a9fb781710826dac4612ed01`  
		Last Modified: Wed, 11 May 2022 12:14:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba5ef14955f3b9bd0d440f2822916ae53e0f1b2f6b14e153beee7d76353753a`  
		Last Modified: Wed, 11 May 2022 12:14:32 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e07fb930035b07bab12fa0884ca365a166f4daea7a0381eab9daca79f12a7e6`  
		Last Modified: Wed, 11 May 2022 12:15:03 GMT  
		Size: 184.4 MB (184376634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e755ca8fb626b007df942c373effbab340f542bcc06664ac91882b107fdb64`  
		Last Modified: Wed, 11 May 2022 12:14:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c836ecbf961bee3cefa299c38ff175ebd1e34e716254d4d7fca9bb4e201bf75`  
		Last Modified: Wed, 11 May 2022 12:15:22 GMT  
		Size: 84.4 MB (84352658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654dee57c72c81b3daef7a0586abe78cc7441000a79c6099794f49ca37c3056`  
		Last Modified: Wed, 11 May 2022 12:15:11 GMT  
		Size: 311.4 KB (311427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027fb463f7c52c796bc55440e7d6c88a0914bd609dd0cc6edf2602adabc25254`  
		Last Modified: Wed, 11 May 2022 12:15:21 GMT  
		Size: 73.9 MB (73864888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcfb9066926d6611cfc2208ca8f0f650d35b8df6780cc869c115cb997753c51`  
		Last Modified: Wed, 11 May 2022 12:15:33 GMT  
		Size: 21.1 MB (21105756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
