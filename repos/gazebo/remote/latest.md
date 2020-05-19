## `gazebo:latest`

```console
$ docker pull gazebo@sha256:900a78c21f122578d77c24f2c516b3680267f726273307c9d39afce5e9c52dd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:1f0df531ff4cd71afb201a9c1eb571275c50dbf663a5b3909714324c0dc3a429
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.6 MB (569632180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:066b13b76596762407dc281b7932c0cbced2cc98bbe058fc29f13a888b840a5a`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:46 GMT
ADD file:a58c8b447951f9e30c92e7262a2effbb8b403c2e795ebaf58456f096b5b2a720 in / 
# Fri, 24 Apr 2020 01:07:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:51 GMT
CMD ["/bin/bash"]
# Tue, 19 May 2020 18:42:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 19 May 2020 18:42:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 19 May 2020 18:42:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 19 May 2020 18:42:57 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 19 May 2020 18:45:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 19 May 2020 18:45:29 GMT
EXPOSE 11345
# Tue, 19 May 2020 18:45:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 19 May 2020 18:45:30 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 19 May 2020 18:45:30 GMT
CMD ["gzserver"]
# Tue, 19 May 2020 18:49:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d51af753c3d3a984351448ec0f85ddafc580680fd6dfce9f4b09fdb367ee1e3e`  
		Last Modified: Fri, 24 Apr 2020 01:09:34 GMT  
		Size: 28.6 MB (28556247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc878cd0a91c7bece56f668b2c79a19d94dd5471dae41fe5a7e14b4ae65251f6`  
		Last Modified: Fri, 24 Apr 2020 01:09:27 GMT  
		Size: 32.3 KB (32304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154df8ff9882934dc5bf265b8b85a3aeadba06387447ffa440f7af7f32b0e1d`  
		Last Modified: Fri, 24 Apr 2020 01:09:26 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee5db0ff82f7aa5ace63497df4802bbadf8f2779ed3e1858605b791dc449425`  
		Last Modified: Fri, 24 Apr 2020 01:09:27 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e5de01a1b5595882fcb3da54a47556f3d36ac6a4a952bc4d2432a0715a4ad`  
		Last Modified: Tue, 19 May 2020 19:01:20 GMT  
		Size: 1.2 MB (1174766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec853c629b8f002231d0b7b73fba8ca49a5c821623e3223dcea449121ffb957c`  
		Last Modified: Tue, 19 May 2020 19:01:27 GMT  
		Size: 16.1 MB (16119110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d634a8cd715762a2a88ed0536fd468bc1d3562c0c8e425b3a119808dcabb71`  
		Last Modified: Tue, 19 May 2020 19:01:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08fc0fe3f8123956179480f973a0daec67da34c81ec808ba03ec7a3801cebb7`  
		Last Modified: Tue, 19 May 2020 19:01:18 GMT  
		Size: 5.5 KB (5468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0089a69352a15fd7b625d79e0b253d3ecbfe84a45890920c4fbb132bdbc22289`  
		Last Modified: Tue, 19 May 2020 19:02:19 GMT  
		Size: 256.8 MB (256806424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b9cb1937f0b78939face34c5bfd4c1fcdfa32419675de133cb62de18956fc`  
		Last Modified: Tue, 19 May 2020 19:01:18 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479cd7572f9315d603d1b31bd2ff0e6fb9265b962b9f338f854be20f282dce79`  
		Last Modified: Tue, 19 May 2020 19:03:57 GMT  
		Size: 266.9 MB (266935229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
