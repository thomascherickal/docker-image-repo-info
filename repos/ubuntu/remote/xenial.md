## `ubuntu:xenial`

```console
$ docker pull ubuntu@sha256:ece75046678ccc064f7f435acf6156bcd0ba8e9525935fa90dc91c249e27fd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial` - linux; amd64

```console
$ docker pull ubuntu@sha256:cc4755a9f2f76ca73055da11f1bdc01d65ce79202a68b041c67c32770c71954b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44402566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab5e942c505d079974d0bb27608d178568973389fd6aadc72c383dee53148a1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d82b1394532561cbab72c86a0da2b66f578e99974cbe147935a3cacdd1942119
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39001218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d186976a24864e6a271dbe9ff152032a3993f458004be2de45cb7497831222e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:09:46 GMT
ADD file:e1ea86c274b93d0a0aa1432f0c9ca1929b7f762085e2298e2d419a2e6765a40e in / 
# Mon, 06 Jul 2020 20:09:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:09:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:10:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:10:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:be0d01e22a1f0d428dbbe6be2da34bbdb47878547862e614fb5eac9a9dc17cae`  
		Last Modified: Mon, 22 Jun 2020 15:53:01 GMT  
		Size: 39.0 MB (38999681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760e2e684f25b6d807a37487630e4b7c8ea9a10ea0272b499fb9ad58a4741c`  
		Last Modified: Mon, 06 Jul 2020 20:10:40 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bcafb819cb1e8d340ca68bdf919d156cde5bb998a5b59d3bc8db1c6c1ab55c`  
		Last Modified: Mon, 06 Jul 2020 20:10:40 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa652f3eed9bab728c77e9d6c0ec8cedd781d52cfb2a75b30ba9e4340b4d6c6`  
		Last Modified: Mon, 06 Jul 2020 20:10:40 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d15b38de5220496b50e2b9d9f2d72d5425a01b991a3e776569d0ae6febd82f41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (40036963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7eddb8de0ef396d0d796256ba2fc254db6cbb7f237d39af1cf7194481f82248`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; 386

```console
$ docker pull ubuntu@sha256:ea9f9fde6a023145c143db5546e03439aef953cdb120154a44fb6d6c2b6a354e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44309561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032561d1b1b13cfc7d45b69eb922b7d469020682f7602a0299b511840af082cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:38 GMT
ADD file:0281a09e4b674b2f3a51152f0248e69f839a107f4f471cb0f27eff2b47ab726f in / 
# Fri, 24 Jul 2020 14:40:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:40:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c0e0b433333915e5da26fd00978221162b377102e5592ae0404898aee9034774`  
		Last Modified: Mon, 13 Jul 2020 15:54:54 GMT  
		Size: 44.3 MB (44308027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe61969407896fc6a99d8afd1014a71214e79872ad515cb536fb625f179bbef`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058d18b29821b7997f08813144585afd758722b51207239ee260207de7afbc9c`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c34ee61901e83a038c1c1b44b6fa3e2636045fa919ae5ea8b7b37020e71ae`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:e5ec578bd8c334d7c9849fd9bbaa78ec25f2b51b0bf7c9e18b1e9b7ca32d6681
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46213021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8ff96d89d56684a658e9b6a3c3891de598dea918df7286e1440bd359ab1f71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:02 GMT
ADD file:dcd2851859d61fd28750e405e189b57c4be98decb40630483b321127e70c7e09 in / 
# Fri, 24 Jul 2020 14:39:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b63cedd79494e27389a6587d305305c6405fd695b4ec7afb75d1f68bf207ef26`  
		Last Modified: Mon, 13 Jul 2020 15:56:00 GMT  
		Size: 46.2 MB (46211522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78d9771dc7acf0b6f60d469c9b7a9e77989fd64a0b0efb42e1f33bafd86065`  
		Last Modified: Fri, 24 Jul 2020 14:43:33 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed6828e9eba3a3a47f543b8e5cd196fc712376d35e3b4eb322896a90501447f`  
		Last Modified: Fri, 24 Jul 2020 14:43:34 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5111fc2327dba7ff082661e123c7a3589ad2d5cd4dcc2588f1eefc61c8162f4`  
		Last Modified: Fri, 24 Jul 2020 14:43:34 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; s390x

```console
$ docker pull ubuntu@sha256:91c8408fcd69b67621810e2787ab8f661a7449ee2f7a0133f0b0771dcb0b1091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42931004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9fe172094fed28581ee6cb7a799cfabb4076d2445205b27336147f780e7a9ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:45:03 GMT
ADD file:bf2a54d719510136249335d267c595d8495031cf3ed3d69c9975f05444bb5129 in / 
# Fri, 24 Jul 2020 14:45:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:45:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:45:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:45:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dbf86c3f4bdb4fdbb59faf631c0d05be1eb33fe938b6332ee07ab035db0a4f8e`  
		Last Modified: Mon, 13 Jul 2020 15:56:10 GMT  
		Size: 42.9 MB (42929517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ce80f41f1cfc5a98c8078530c4618f86fa77832bdf0b0bb484211359473956`  
		Last Modified: Fri, 24 Jul 2020 14:46:17 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdadef093efdb822d71f1ac71a76f40485cac65269a99e6cb366a8fd5548f7d`  
		Last Modified: Fri, 24 Jul 2020 14:46:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f849fe87969087a98487dbc416d25c3dda1b7f7aae893a93963b8615ca8b7903`  
		Last Modified: Fri, 24 Jul 2020 14:46:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
