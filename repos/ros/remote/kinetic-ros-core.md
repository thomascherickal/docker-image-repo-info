## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:4c50aa6ef165d8cafaba5f5995de52ccd2c01eed7b48f979eebb1f699c2c4008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f79f3508b9b3d12921c59db9a4fc31010eb1667fd690d9da937c451ffc9f98b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243917932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433fb8323bb93515f0dd182b03f5eeef64906471c3f0f147e717f38df397d028`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:39:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 21:39:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 May 2021 21:39:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 May 2021 21:39:28 GMT
ENV LANG=C.UTF-8
# Wed, 19 May 2021 21:39:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 May 2021 21:39:28 GMT
ENV ROS_DISTRO=kinetic
# Wed, 19 May 2021 21:42:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 21:42:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 19 May 2021 21:42:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 May 2021 21:42:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14684ba412c39757a989fb7fe7e1858ffaecf276e3190ccd4765dabe7a1e8b11`  
		Last Modified: Wed, 19 May 2021 22:09:00 GMT  
		Size: 5.4 MB (5364316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d57d18c871aa3698dca1c280246f6e78f80e39a8c306763750d9fdce93efff`  
		Last Modified: Wed, 19 May 2021 22:09:00 GMT  
		Size: 14.7 KB (14746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea861d8af8441bf794d8e6e8770d22b11cec75699560edff78932dce34e29a83`  
		Last Modified: Wed, 19 May 2021 22:08:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39413ca8ec49abf567b8c4497755073cb268ea3568fbe548b86f454849e3566d`  
		Last Modified: Wed, 19 May 2021 22:09:30 GMT  
		Size: 192.1 MB (192075126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3d8fde9915f7333a8aa902f390231c5576b7f801aff8f872367f5531572170`  
		Last Modified: Wed, 19 May 2021 22:08:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:649b0bea05e86fb950bd4a9839b5d551b60277ba00512775a20af4c918043206
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216901865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7096c1eaedaa8e083894b1a555733e0cb7b7ecc8f71abb574fa43d7c148aef2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 May 2021 17:01:40 GMT
ADD file:7e5c1f0262200ed290a61913d7f2c3b2b064c9b02aa1a55a818e38ab1316bbda in / 
# Wed, 26 May 2021 17:01:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 17:01:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 26 May 2021 17:01:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 17:01:42 GMT
CMD ["/bin/bash"]
# Wed, 26 May 2021 23:52:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 May 2021 23:52:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 May 2021 23:52:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 May 2021 23:52:36 GMT
ENV LANG=C.UTF-8
# Wed, 26 May 2021 23:52:37 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 May 2021 23:52:37 GMT
ENV ROS_DISTRO=kinetic
# Wed, 26 May 2021 23:54:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 May 2021 23:54:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 May 2021 23:54:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 May 2021 23:54:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ae1370da0037e05eb3f24cd486c49ee3a450840763c7d31deef8274cb9abfd86`  
		Last Modified: Wed, 19 May 2021 20:24:51 GMT  
		Size: 40.3 MB (40292258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f08183c6e31c7e342a25706e54f9869aaf760990cb4a4ccbd4ed8aa917076c`  
		Last Modified: Wed, 26 May 2021 17:05:29 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5e978cf38433440cb631931ba431ef9da5d6e3ee162ca67891562db1df11af`  
		Last Modified: Wed, 26 May 2021 17:05:29 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4087b5e6a0394da1cbb5e8e721ff4d4cb511d79e6a83e7e1d84ed9352de6aac0`  
		Last Modified: Wed, 26 May 2021 17:05:29 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33faccb4c2f61c169e577fcfdc727151dd9b03ec93da6e0fca01674d95cc322f`  
		Last Modified: Thu, 27 May 2021 00:21:41 GMT  
		Size: 4.6 MB (4615749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f6e9c01108a0f8f16fd0ce8d6c5a20f0852da78cb8365cd092def0bb6852f8`  
		Last Modified: Thu, 27 May 2021 00:21:39 GMT  
		Size: 14.7 KB (14745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a02f61386a0196c1c99f7458202856ace3934e6b5d5cb394e079db5363f345a`  
		Last Modified: Thu, 27 May 2021 00:21:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb01c41b95a6205f484a9dc3c089458d5e38b1707af7b3f01135f72bc7b93ab`  
		Last Modified: Thu, 27 May 2021 00:22:38 GMT  
		Size: 172.0 MB (171977161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca5fd0bb4c103d17b24eb900b0d32c3e9fcc35ca9976e420e5e5f648b68f569`  
		Last Modified: Thu, 27 May 2021 00:21:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4cb2d5e8a31c353a61ffb16696f45bd5696b7c25b0c16d6046f6d09bde18290d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226155857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9b2a86164b5cc5b965f44f37037987afaa1493f6a42e0f55988052930d3fbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 May 2021 12:30:43 GMT
ADD file:9417aaf175748bf02265b3fcffc4955c5521d4d51793d599f33e48b7960e453e in / 
# Thu, 27 May 2021 12:30:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 27 May 2021 12:30:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 12:30:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 27 May 2021 12:30:46 GMT
CMD ["/bin/bash"]
# Thu, 27 May 2021 14:56:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 14:56:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 27 May 2021 14:56:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 27 May 2021 14:56:40 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 14:56:40 GMT
ENV LC_ALL=C.UTF-8
# Thu, 27 May 2021 14:56:40 GMT
ENV ROS_DISTRO=kinetic
# Thu, 27 May 2021 14:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 14:57:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 27 May 2021 14:57:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 27 May 2021 14:57:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:58be9ce6be6955598846443a55535df82ab8b8489d8a09eb959abd45a368503b`  
		Last Modified: Thu, 29 Apr 2021 08:25:11 GMT  
		Size: 41.2 MB (41212503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2536079c067c30e81c2fd80224355786c22f125638814e45caa9357de3b332b`  
		Last Modified: Thu, 27 May 2021 12:33:41 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1407aa15569186ac220ed788ef58c2821961717f50af3355e9302617acddbfb`  
		Last Modified: Thu, 27 May 2021 12:33:42 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566efc3b50d0a162192bf9a472fe8ff4e3d7be9791f42b800f9475188301ecac`  
		Last Modified: Thu, 27 May 2021 12:33:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6001bc3508e18cd183c46954464ce088871f8b5037c36b0bfa1e19a2766b1f83`  
		Last Modified: Thu, 27 May 2021 15:34:19 GMT  
		Size: 4.8 MB (4820841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992e851dcef7358f9fce0c8b498702d4d19c8f314694b14889c064acf1662c70`  
		Last Modified: Thu, 27 May 2021 15:34:18 GMT  
		Size: 14.7 KB (14744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f30a742187ee56990d6c615e1be3966d99d5fc44b8b6fb714c88d181c7f48`  
		Last Modified: Thu, 27 May 2021 15:34:18 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b71daccc6377eeffa55a6047c88a788a9bbaa88855afc6ceb106facb716f5d`  
		Last Modified: Thu, 27 May 2021 15:35:03 GMT  
		Size: 180.1 MB (180105859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06b779cfaea72e43ba42219acd071be27631bd84788cfe5f892a3b80554756f`  
		Last Modified: Thu, 27 May 2021 15:34:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
