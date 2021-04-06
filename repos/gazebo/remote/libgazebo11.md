## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:3e4ff757ffafbb76b263aa53d35c15331ba414772a357f909ccd8713c853f0ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:4d5d0ee0ea8dfbd97b7e9315def9f4303685d227c0b02b03ee4eef19be610c0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **598.7 MB (598658052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d988d54294fc0b35d75862d2c8654e2782ee7c6db31d7764c99dc0d067ce8933`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:08:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:08:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:08:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 03 Apr 2021 02:08:28 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 05 Apr 2021 17:37:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.4.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Apr 2021 17:37:19 GMT
EXPOSE 11345
# Mon, 05 Apr 2021 17:37:19 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 05 Apr 2021 17:37:19 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 05 Apr 2021 17:37:20 GMT
CMD ["gzserver"]
# Mon, 05 Apr 2021 17:42:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.4.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c5d2d7a6606006c3c9ad68491e77516419c59fceb2f4c04ca5580c96d8501`  
		Last Modified: Sat, 03 Apr 2021 02:40:16 GMT  
		Size: 1.2 MB (1182070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0433c00a288f1240767f1d7d9266f8d29483e0261a28d2da525efe48551ccc0b`  
		Last Modified: Mon, 05 Apr 2021 17:45:33 GMT  
		Size: 16.1 MB (16148865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18635ab6eb1ee4fa0dd36232501ac15454559ccf7f76145cd95f76c8c4bd357`  
		Last Modified: Mon, 05 Apr 2021 17:45:26 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb6bc01d63fefcc47e74a13105096e0103b5f4ce5a5583ecdcdf65888b1ada`  
		Last Modified: Mon, 05 Apr 2021 17:45:25 GMT  
		Size: 5.5 KB (5498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2f15ef4a701685efe82a50719a5dfb7eaa45fe0e502ba8f69cade4851e0b1b`  
		Last Modified: Mon, 05 Apr 2021 17:46:17 GMT  
		Size: 272.4 MB (272376622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c531604249ce6063f468a26abbdb66d343ef333e3fddeb26c4df630ccdc7edbd`  
		Last Modified: Mon, 05 Apr 2021 17:45:26 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d29c39b24291bff7e6bc96c1bc63ceab09dcb8d02846de4ee759ad0c9cec90`  
		Last Modified: Mon, 05 Apr 2021 17:47:26 GMT  
		Size: 280.4 MB (280373317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
