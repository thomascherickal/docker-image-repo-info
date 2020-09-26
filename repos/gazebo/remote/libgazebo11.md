## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:9f7d04702851ad30921aaccf67c33d47e0cd5376e68a351a6ee19c128f386fca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:afb4321c652741c175bb4b6b99911806dca41246029b791e132986e6333a0bb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (590037713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0d069958d144bfcc76791a9a1630f0a340e85112a03cb0b2235c750aea985b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:13:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:13:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:13:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 26 Sep 2020 00:13:57 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 26 Sep 2020 00:16:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.1.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:16:35 GMT
EXPOSE 11345
# Sat, 26 Sep 2020 00:16:35 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 26 Sep 2020 00:16:35 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 26 Sep 2020 00:16:35 GMT
CMD ["gzserver"]
# Sat, 26 Sep 2020 00:20:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.1.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac7e7e50c4ec78d366977925188b5bcceefc778ad809bbacacfddc2494cf44d`  
		Last Modified: Sat, 26 Sep 2020 00:33:06 GMT  
		Size: 1.2 MB (1176627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79faefb2969cc6c5da0f5cc5494d1df5ec1fd1851f3cc49b9ddbe719be383124`  
		Last Modified: Sat, 26 Sep 2020 00:33:10 GMT  
		Size: 16.1 MB (16116950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cff56dff73ab02e30c6734e2e8c20c97df4d2ee4ee7b2c43e524ca4d8e010a8`  
		Last Modified: Sat, 26 Sep 2020 00:33:04 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f18e86760e1d105ffea1ea5f63eddba4c58251a2f0dcb8c98e6cc7e2d29a01b`  
		Last Modified: Sat, 26 Sep 2020 00:33:04 GMT  
		Size: 5.5 KB (5471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2538a4cf2b2dc32db8633b9bf6bcadf83240bb397baf7a355fc2e32a1dc495ef`  
		Last Modified: Sat, 26 Sep 2020 00:33:44 GMT  
		Size: 267.6 MB (267569223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300f2f76743429b7943cfe31685af1b705efc2790949af2579fe7c59c1186c90`  
		Last Modified: Sat, 26 Sep 2020 00:33:04 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6c5b09662c7f4e6e65e2d46c978f3302a17c9381f3577b07262cc945219e47`  
		Last Modified: Sat, 26 Sep 2020 00:34:57 GMT  
		Size: 276.6 MB (276608760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
