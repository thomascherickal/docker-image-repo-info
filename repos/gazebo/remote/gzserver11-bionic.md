## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:99d0a6be935f601cb3e274c50ced99f76ef001be01fc707b6bd4051849d54d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:14e94b30f1aab6bbb7c02577d77db667cbb1790b104ad05c9d5e7cec2fbc9d11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301472383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c4917ccb156fe3d7badf132bb0c0109eb5d6c69ad34b7f159ed413557786a8`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:02:45 GMT
RUN apt-get update && apt-get install -q -y     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:02:46 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:02:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:02:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:02:47 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998f7e37ef010e3138493d5604da592ef98e7e5758a0111e1a4645212a099e6`  
		Last Modified: Fri, 20 Mar 2020 21:08:22 GMT  
		Size: 258.7 MB (258749521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db145bf1e587e0089f1dc4d6f46a371c077701f8506db0f75025db663e118f6c`  
		Last Modified: Fri, 20 Mar 2020 21:07:44 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
