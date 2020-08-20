## `buildpack-deps:groovy-curl`

```console
$ docker pull buildpack-deps@sha256:4ee2ee2121b83e0ff2b41b380f598c128409abe61bfc24623eed41b17f6e85a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8bdabf86543b9ce5dde126c0a98102943e8fb4d6df8437294970ca17053fc380
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39291079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2898054052936c529e7c0eb288d2b3286dbde156521abb648d02ff8a6f16e92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:15:22 GMT
ADD file:53ca8a3f446b0751019d522066ce844f6281ffb5b15e9605cd8940176abf4c76 in / 
# Wed, 19 Aug 2020 21:15:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:25 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:27:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:27:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d94cf711eb1df9e05b5ab9c367f7417c481e9b5deee1724f93b96c77bff11c8f`  
		Last Modified: Mon, 17 Aug 2020 15:53:01 GMT  
		Size: 28.8 MB (28809294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc1ea4c1ef986e00d114cccc9e5fbbe6bd5b8f35145cacb0f12ae3389c4e0a2`  
		Last Modified: Wed, 19 Aug 2020 21:17:10 GMT  
		Size: 31.0 KB (31042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2147ebd301d69260017329191f4072fbb193e2c1c092542270947091c6eaa60c`  
		Last Modified: Wed, 19 Aug 2020 21:17:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2955d4b7554096a19ae03fac9a539a3106b871165d9beef32fb6f3b16bed6c4a`  
		Last Modified: Wed, 19 Aug 2020 21:17:10 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff92321eef344d6f7de248e128d72b31e764780d34efaa3ddd1379ab12aed1e`  
		Last Modified: Wed, 19 Aug 2020 22:36:01 GMT  
		Size: 6.9 MB (6863303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378b1e0fc390f4096ef8d0f7e763d0862ec62b697cf1bcc6e89a0e73fa780949`  
		Last Modified: Wed, 19 Aug 2020 22:36:00 GMT  
		Size: 3.6 MB (3586428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:394f2561223c03e8e260500366143c875bdf7f005a763ff82eff20a602ae4961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33146336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d240216d999088d25a277e118411bf991a7d8fd8c5d40fa7cfb721fe59ce19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:46:00 GMT
ADD file:0bf418503e730b1c07a5f7cfa6bb46ee5632cc7b373b62ee6dd516fd9ac74a74 in / 
# Wed, 19 Aug 2020 21:46:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:46:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:46:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:46:08 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:42:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:43:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51f59682918cc084f352717f5c3396b728b9330e743eeb2b4e68dfb462af45d7`  
		Last Modified: Mon, 17 Aug 2020 15:53:50 GMT  
		Size: 24.2 MB (24193556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b1422315ef362739026a4ca046b2e2d8c997dd3e3abb96a1be02059d277f54`  
		Last Modified: Wed, 19 Aug 2020 21:47:41 GMT  
		Size: 31.1 KB (31088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5e75f32a143c512dd9eac32b387a755f89cce7c5ba380f97e7925c151578cc`  
		Last Modified: Wed, 19 Aug 2020 21:47:41 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad5a87e6717b17b109e7c4181ce3bd137895c7b03457c41fde02ce7ccbcb69`  
		Last Modified: Wed, 19 Aug 2020 21:47:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5c4e5df9a2ce3762133a9238e4c83e6a984aac91089157e4fcac17d461c339`  
		Last Modified: Wed, 19 Aug 2020 23:56:47 GMT  
		Size: 5.9 MB (5861346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3155a6136369da11d20f340e0774bfbbf9796bccd017b2e527ab247d2101399`  
		Last Modified: Wed, 19 Aug 2020 23:56:46 GMT  
		Size: 3.1 MB (3059313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f49f252d95d4707a3f527c6c8730dd9875d1188dfc7bb1d9a8c29b9c39c3e7cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37741851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7126dd3b44a59c3c32a4661ac47c70bf43a82b43e93da0418d8b5aa830a42e7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:30:48 GMT
ADD file:a2368478f6147dfb550f11fd08fa580527841837e6de780105b0ee3c869e9045 in / 
# Wed, 19 Aug 2020 21:31:01 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:31:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:08 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:06:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11602f8d9ef9a64d301368c826db17ed80fdaaa6895c8479600ecfb22906feec`  
		Last Modified: Mon, 17 Aug 2020 15:53:49 GMT  
		Size: 27.4 MB (27411937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9baf34eaf014c357d3680a1c3659aa57594a0cf1e8f13f3410ff6e659147f0`  
		Last Modified: Wed, 19 Aug 2020 21:32:46 GMT  
		Size: 31.0 KB (31023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f4efba19094c2a8cdccdb0aad9f813a4ae4c9ecbb8028522dfe7136037188c`  
		Last Modified: Wed, 19 Aug 2020 21:32:46 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61503eacf6a2d668185f96d1697af41f5c1798343a4903c2141b75db7ba35fb9`  
		Last Modified: Wed, 19 Aug 2020 21:32:46 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959af42e9a96454cf5f9d0df1902056102efc1f8c5fce06fa385fc6234dc4e18`  
		Last Modified: Wed, 19 Aug 2020 22:14:37 GMT  
		Size: 6.7 MB (6727192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74393685c57568d31f3de5b52a660d8f421b7493deab4a65599fc6cafa475491`  
		Last Modified: Wed, 19 Aug 2020 22:14:37 GMT  
		Size: 3.6 MB (3570662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f03f0e1c43b8d0bcacad1076dfac435f16b82b4d2df77b551d7f36d15e5c95a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45247850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a52b302f9dbe0ddc8f4552cabf964492309d21139cf82595ddca4c24ed9be115`
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
# Fri, 24 Jul 2020 18:29:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:30:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
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
	-	`sha256:f316702b922618a7a9bbe6a4ba46d737e166db8c781e15bc3e62b7895e72a4aa`  
		Last Modified: Fri, 24 Jul 2020 19:20:00 GMT  
		Size: 7.8 MB (7815065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62398f1446e8445ee9f855bf3fd20e927777bc1267fea9901b7204bd161a0f5`  
		Last Modified: Fri, 24 Jul 2020 19:19:59 GMT  
		Size: 4.4 MB (4447440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ac60029b2ee4e5bd2ceb496ce6365e642de56b4effd2a6f04edde29d4cbb63b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38736655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e3005e81a4cf67155d241a32918779c8a09eb57d8d07085b92a03b3a068a04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:31 GMT
ADD file:62afc24038998372a88abab1eb3c5eddd0c6551c6e5c56eb3f466ca26816e9c6 in / 
# Wed, 19 Aug 2020 21:10:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:37 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:48:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:49:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:920f4fc5f9a3eec734000cb609b35bce4bd842b886967e3f9242e9b1ef4c1851`  
		Last Modified: Mon, 17 Aug 2020 15:54:28 GMT  
		Size: 28.5 MB (28545182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b78dfbe3669075931a4f4250923d05bb9ee9276049becd7b75122e444faceb`  
		Last Modified: Wed, 19 Aug 2020 21:11:34 GMT  
		Size: 31.7 KB (31719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e366567dad155c04eedb45feb0b4c6afbb4832bac8ae3a9e60d49bf795c0d8c`  
		Last Modified: Wed, 19 Aug 2020 21:11:34 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa80c73ca70349d062cdd34084bd45aa84f9e86a5b141ca7244b26ec6e436590`  
		Last Modified: Wed, 19 Aug 2020 21:11:35 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c94bf7f800b71eb421372b72a3176ba745cd9cbc1566dfaf73b5ca3a59eccc8`  
		Last Modified: Wed, 19 Aug 2020 21:54:05 GMT  
		Size: 6.6 MB (6579239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d158b1fc9747cfc0d5b50d7a6071454547d69a2862eac4ff89ddf09fea57c99`  
		Last Modified: Wed, 19 Aug 2020 21:54:04 GMT  
		Size: 3.6 MB (3579486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
