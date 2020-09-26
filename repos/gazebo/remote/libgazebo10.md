## `gazebo:libgazebo10`

```console
$ docker pull gazebo@sha256:994de1a95374b5d784d7a28c2db6357b208802f73595300cc04ad54fceefc789
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10` - linux; amd64

```console
$ docker pull gazebo@sha256:02e4c1caeae30613c33b1de2a388d0cd7b404334b83c3cb87ff9832b89d25ee6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.1 MB (522052897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbf1bdd1b1d4e60ff325f179beb3f3f2f1ecc31a9722f7bbcb07759bb331abc`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:03:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:03:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:03:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 26 Sep 2020 00:03:36 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 26 Sep 2020 00:08:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:08:54 GMT
EXPOSE 11345
# Sat, 26 Sep 2020 00:08:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 26 Sep 2020 00:08:54 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 26 Sep 2020 00:08:54 GMT
CMD ["gzserver"]
# Sat, 26 Sep 2020 00:10:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e9ed312e3419a4c4db0767b3098eb605e89291c6ec52e2a1f9267e0d4e036`  
		Last Modified: Sat, 26 Sep 2020 00:26:41 GMT  
		Size: 838.7 KB (838713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b54a8c04d64037cbc7c27376d62f9de9ad653485d273ef711b9fdf7ad474e62`  
		Last Modified: Sat, 26 Sep 2020 00:26:44 GMT  
		Size: 14.7 MB (14698148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ad9c6ab10be6e9bd4466a06c68a4e06e8e7de8a8ab0c4a6d9b20f6f978de66`  
		Last Modified: Sat, 26 Sep 2020 00:26:40 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8074a5819c7b3a89ab71255cb5d43827d6260ffcd2a1b457557183a461e1dad`  
		Last Modified: Sat, 26 Sep 2020 00:26:40 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0588d62da7ea46dc613e79ea352d8733af3d0e77ce874addc3223f31047641`  
		Last Modified: Sat, 26 Sep 2020 00:29:09 GMT  
		Size: 226.2 MB (226170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb225dbdf3ea03fb7756fcddc464b5c1bf64dcf9130f01a897acfbfb35ee3e25`  
		Last Modified: Sat, 26 Sep 2020 00:28:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581150d7c579ab3e3eff68904745b2e08f1c8f148484d71e30188cd540e45ae8`  
		Last Modified: Sat, 26 Sep 2020 00:30:08 GMT  
		Size: 253.6 MB (253635694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
