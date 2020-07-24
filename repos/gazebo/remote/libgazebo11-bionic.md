## `gazebo:libgazebo11-bionic`

```console
$ docker pull gazebo@sha256:97e27d9f82e90d8fd5ca34a7a885e0aaaad1c748a17c5a8718ce31dea6acaef8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:180eb43b0f7da835adb11256efd8449349f027d6b1368bdb2aefd2c2f1238906
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.5 MB (531507725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7e25d23a2b1f9aa9d7cd1e001927a4f148b307cd0f0cfd21345b5db51724af`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:53:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:53:20 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:53:20 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:53:21 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:53:21 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:54:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d336f5ab998002a7fd27f7f97823a79da33db94abf32261ea0c04540821434bc`  
		Last Modified: Fri, 24 Jul 2020 16:08:35 GMT  
		Size: 227.6 MB (227622485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479035b2b323db88d46c9c942312551f91f9ddc329bb79cf9346cda8527bbe6e`  
		Last Modified: Fri, 24 Jul 2020 16:08:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb199665193c7552b70e9b701641ee3821ea675406a285d9592bb0e079cb74b3`  
		Last Modified: Fri, 24 Jul 2020 16:09:32 GMT  
		Size: 261.6 MB (261611538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
