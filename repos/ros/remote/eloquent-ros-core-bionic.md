## `ros:eloquent-ros-core-bionic`

```console
$ docker pull ros@sha256:8c4adab1942f0bd633e1c71fd2760e43e9f6690d5f8a0c48980df8f412fa60aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b25002a9a59837256e9b3f4872007324458a7b87145637a1477462b2ac62019f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215371732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b701b84b9498423d722b05a99c147293234764bd3125e926ef31cac8b5264715`
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

### `ros:eloquent-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ccd5eced9c79fbc16c7dd15cccfa36bf6ab7caf168b5ebfa873a100d7965474d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183769963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982e08903cf1512355b29fb9cc8c8f8a028cf8cdcfa8b9ec70ce6ebf651b5b33`
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

### `ros:eloquent-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:45b9dc7ba449fd205637cfcd35a6967c6930c6a3d5f9f018221b008cca37308d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.4 MB (197386467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bbf629c60c34bf8a541bbd3ff5e58acdbf4827d1f81ea3ae835a2cdb01874ca`
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
