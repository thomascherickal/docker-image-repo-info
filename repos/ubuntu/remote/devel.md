## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:3aee55358bbbfc95e1059341f08fe5f448eb93dcd746365be39597d011621e47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:2fb1f8af49f296081dd4fbf33f3f0c5da3be8dc4c413bb6545628f086c0f6408
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28390799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:188e030eedba1500bd3082eece304c1ee29ac38affada33744f4208cb4248596`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:45 GMT
ADD file:8cda7bfcf6c3010f9498acf5db465d8affd86bacb786338974486e23ea62b05d in / 
# Fri, 24 Jul 2020 14:38:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5f55bfaf77a136f7c6b5063e591480c2e7690ed1c29b0ee354caf8f6c62741e0`  
		Last Modified: Fri, 24 Jul 2020 14:39:44 GMT  
		Size: 28.4 MB (28357957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef373180da2631c7a56d9629e37de8010fe57414453617dde3a2c1e9861f1eb`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 31.8 KB (31838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d10b513df5337d26a6e2ccaf4875267999084d7f0d2f3102c54d7430cfa35`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552f92805e8c6585c466083ac60f40092ae127e794d498c599a31bd67df21c09`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a53bdcdaf1f7d23a4a26ed5b90e825eac17c8e1c31280ec1a46eda5284b2429a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23879702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d9420d2b6c86f2abd89a6e5ffad99897d7b7517e3eb5339b1ccd0c3d950b2a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:08:43 GMT
ADD file:021612df98a3252c0018261734979dffe9cdc59bdd68707ae03cea58d0c65498 in / 
# Mon, 06 Jul 2020 20:08:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Jul 2020 08:04:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Jul 2020 08:04:54 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Jul 2020 08:04:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:008c40b75c61a21ea627c86505f910d9a47056dc120ce6996c3d080b08658308`  
		Last Modified: Mon, 06 Jul 2020 15:50:47 GMT  
		Size: 23.8 MB (23846810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669074342c885ac270b199e748002596d0f32df7f77c659f5413f77f274cc91e`  
		Last Modified: Thu, 23 Jul 2020 08:05:45 GMT  
		Size: 31.9 KB (31856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6860323f7121ae3ef42c0e5a729d9019a7d73fb9243d8a51943a2aa107c6b7`  
		Last Modified: Thu, 23 Jul 2020 08:05:45 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afad5102492ecbe7ecd632b6fe604a800b86c249d9d2b3479b2da9647a22495`  
		Last Modified: Thu, 23 Jul 2020 08:05:44 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b641398f9efbfe15df2fe68d3d9c3050a300ce7f71ab1f4df37c4ddea9bf52ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27002111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f5cef8c4497db22aea98cdedc946c0a3cafb462096d4f23548194288fd5ef4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:05:50 GMT
ADD file:35b0d977e8fc4305b3f988e3af2c52419e39aae68287af590636dfdb7487dbed in / 
# Mon, 06 Jul 2020 22:05:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:05:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:05:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:05:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bca3f99199d9260076c548f38af71788f901900c99316e357c1dfb0e06fafbd6`  
		Last Modified: Mon, 06 Jul 2020 15:50:50 GMT  
		Size: 27.0 MB (26969246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf01b6284862c6caa2ce0e716ddb00705d21bb4f7cc4501c1fdf1130c17ffa7`  
		Last Modified: Mon, 06 Jul 2020 22:07:25 GMT  
		Size: 31.8 KB (31830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e991f38a848885cf9ff0e35cb51871c37ee33387f3159b4dbd1fa25146a3ecb`  
		Last Modified: Mon, 06 Jul 2020 22:07:26 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b128a6106c13f4424dcc44fef4eaa219acaf5f3c8510660e77bd90c81e6227`  
		Last Modified: Mon, 06 Jul 2020 22:07:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:027242691f288b0770ec88389e9643f7141ac61200396a2a890795c43223a56e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32985345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29933d6f8d91ece30bd342f40955af0eaf4b0cce7cb1e5eaddbac7eea91e32c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:37:12 GMT
ADD file:c00451f5cfe44d733a24fd1ed2ffcd58dd03d160b3be1f23a23c6988bfdde5f9 in / 
# Fri, 24 Jul 2020 14:37:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:37:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ef413e40463b2cc51faddfd43a7ccebc442b8f3e610f2099c9b9f43ab4c794c`  
		Last Modified: Fri, 24 Jul 2020 14:43:13 GMT  
		Size: 33.0 MB (32952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a2aa97dce56eeeb38597752e261e49aa1782887302c44ab406af8642599fc`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 31.7 KB (31677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0098b0f09cf883a00d68448733220790bdd0cf13bdbf30b747c84687fa0ca2`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f899dca8f8bc39cfcda10bb89d224e2d1b4dbcb2a0c7d0b2bfd4e11bd11f0f61`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:2c2f1bd5f0e8469d0913dfcf2f5ebb5e0848f6d1a338b3f6444423a2f7257f83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27263645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6579b622c1a85a84003396d344881960164c590e676d704aee0925dcf753c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:39 GMT
ADD file:c2305b9c6b3d1f88851d28a75f00aefa09cd090dceed56cea0be0ef7848de90d in / 
# Fri, 24 Jul 2020 14:44:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:96ee9d07fad79c13f98051a8b3a80c5aa966b8b8e5c86f129811fc3e03c6a937`  
		Last Modified: Fri, 24 Jul 2020 14:46:02 GMT  
		Size: 27.2 MB (27230132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e509548444259d3ffae6be4cff91bdbd942e76236063786c133bd7a9916cb74`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 32.5 KB (32481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45af8f70e0f28da9bf410c9369c787d38fdd7d9bf805098562a6a4aefe14c3a`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13885bcf94b5ef67414fbe9d1bc297ddc27a295f43fef37c3e0b67cb4449003e`  
		Last Modified: Fri, 24 Jul 2020 14:45:59 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
