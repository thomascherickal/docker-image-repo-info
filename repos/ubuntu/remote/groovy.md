## `ubuntu:groovy`

```console
$ docker pull ubuntu@sha256:8eb177672d788f5ee57f091a5d9a927609c1c87278fea4cd919152ee8dc6e0c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:groovy` - linux; amd64

```console
$ docker pull ubuntu@sha256:7e18ee3ffa8f4b65deb0472b0a553ad6d7b07440abc0c8b12859614a18b46b05
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28203286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73bfdffe747eacf5936ca6f390b69fa7640b315b30ae8a8dc7d0dda7379a581b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:05 GMT
ADD file:92952db7a9177df30b622431b9f8fefbcd7a939849c42bf0c4f13bc351e4afcb in / 
# Wed, 17 Jun 2020 01:21:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:21:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0b4f5d796ad9b8be2c7e6e6bf2af20f7c4d7767f09d685031e8d2f74f88aa976`  
		Last Modified: Mon, 15 Jun 2020 15:48:18 GMT  
		Size: 28.2 MB (28170426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee7132703b3afff26639216d0405c82708835c086de365d565d615e3f0921f`  
		Last Modified: Wed, 17 Jun 2020 01:22:12 GMT  
		Size: 31.8 KB (31847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e5b34dda87e71c8d1974483aa2b77b73924fedab54ffe098b2a7c51fa4cf1`  
		Last Modified: Wed, 17 Jun 2020 01:22:12 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3af786f5e76b85e0e94a65a039de3975fc9e68d8bb556a69b78a2b0ac7fda9e`  
		Last Modified: Wed, 17 Jun 2020 01:22:12 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8a88040120a452fb612fa96683c1b0df614bd107560b2f695d4830ffa64dc676
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26809273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edba44d23c4f9ce97c21b38adad072dd27b4bee25f461c48bc470997c86d255`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:43:47 GMT
ADD file:79a5e9ec755c39a63ddb87e95abbaa4e7f58c2b21f6fdc989988bc596132fb0f in / 
# Wed, 17 Jun 2020 01:43:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:43:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:43:54 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:43:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8feffc3ef06df85a0b885c9ed0142729b9b6ab40b1ae0e1c80acf8a166828332`  
		Last Modified: Mon, 15 Jun 2020 15:48:52 GMT  
		Size: 26.8 MB (26776408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1d229880df445d6616abd62f73150dd4f69ec83ea2518df98a22cec7717992`  
		Last Modified: Wed, 17 Jun 2020 01:45:32 GMT  
		Size: 31.8 KB (31828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ebd8c9dbc7b239e6537d01cb2f8917d318937078b6d819e53d9a3a917c87cb`  
		Last Modified: Wed, 17 Jun 2020 01:45:31 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9ddb4021ce9fc1951e508097c3b6a69b56a2c35e4ba359eaf7d34f4a2a7d98`  
		Last Modified: Wed, 17 Jun 2020 01:45:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c327451ed2108692e3134eecc0b3b0ee2d8b02643bd5b820b5503beb7a40d67d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32863904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad81f1807d0b7e50beff1c1fc8f7162a9c34e54bd9740ab1d79e12c12958f684`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:26:10 GMT
ADD file:29a6559bb2b42840ad4a326cb87ec57e3d7acff070142d3c445e95a498608e9d in / 
# Wed, 17 Jun 2020 01:26:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:26:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:26:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:26:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b25075d60966612c3c64d57b4795ad61c96f1b6726b5f4e2bbe9895da022ab69`  
		Last Modified: Mon, 15 Jun 2020 15:49:24 GMT  
		Size: 32.8 MB (32831214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ca039867a3a4d1f0bdce8cd95a4d5cae3bf26445e7da18368ea1a321552ef`  
		Last Modified: Wed, 17 Jun 2020 01:29:17 GMT  
		Size: 31.6 KB (31650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74cdff241e2c333351680e082de3609a7cbaaf2ad00a453b5b11f5d36990e02`  
		Last Modified: Wed, 17 Jun 2020 01:29:18 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9272e5603032808e3b694ab411de4202c12aa58e48b2e449ae98b88773a4684c`  
		Last Modified: Wed, 17 Jun 2020 01:29:18 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; s390x

```console
$ docker pull ubuntu@sha256:8512818c0c072aa98ec80796d24980d02934406a9ff294d66ec7d6394af8a23c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27207601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:305b81ae96a200beaa985bc8e4d48770c732e7a55c6422635b8cd6d4be962871`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:33 GMT
ADD file:7c5297f390515aab00f66f663182cadbb3c5dbf52fb015526b80806df21de69d in / 
# Mon, 06 Jul 2020 20:20:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3c5e60e47f65a4306c7d2ad46d35b9ea6d4aaf9cb77add2bff5be52a742d23e4`  
		Last Modified: Mon, 06 Jul 2020 15:52:10 GMT  
		Size: 27.2 MB (27174117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6ddf166e3f11601f2466edd2cfbfe9942c0f85314ffb2ea31f66bb6d0cf123`  
		Last Modified: Mon, 06 Jul 2020 20:21:35 GMT  
		Size: 32.5 KB (32456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f8572b34a88b603a66fc9eba9b5237c09e64670ac0d8a02e024d6e3ade52f`  
		Last Modified: Mon, 06 Jul 2020 20:21:35 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f928d1948ab604aafd2985aaa9196351c03043dee8e4bbbd73f4cbf190abb675`  
		Last Modified: Mon, 06 Jul 2020 20:21:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
