## `buildpack-deps:groovy-scm`

```console
$ docker pull buildpack-deps@sha256:29861704fe9cc9bafc4fe02383372d5dbcca76bb4d3a6a1d783a6b693771ee60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7133d90d743acf348852f8999198169e563caf5a3a7f3650391bee1bb246b100
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94275718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3a7c6f547ae4136decc8b9a93263163319cc76b543ed16d89c9a0d4a921ec41`
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
# Wed, 19 Aug 2020 22:28:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:403a0f8b5c35d4f809b059fb0d3e8ad6ddb94f7050d41a689fd396fda1b3f784`  
		Last Modified: Wed, 19 Aug 2020 22:36:25 GMT  
		Size: 55.0 MB (54984639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:18e9be63b8f87176dfa75404ae320937c51e3cee518ce4f3d504af761bb14e28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (83026200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85882c6113475ae5b618a67a5ec09fb6df1632fff3aa8aa9ec39feb25b2c135`
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
# Wed, 19 Aug 2020 23:44:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:5ea8decd6ebe983f4d1b2becd7c670468d3ff37e87007b55be943a4df7838f15`  
		Last Modified: Wed, 19 Aug 2020 23:57:12 GMT  
		Size: 49.9 MB (49879864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e606703d00d3c6dbb9c9cef34852e6e4095bdab50883738f23813c8eca8c24c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92748729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44210e04013e14312abc6f2281ed92c83a3462be39ba0a2a9715dcb6f2d5cfc`
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
# Wed, 19 Aug 2020 22:06:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4a9200ef6e477aebe4b7e791f3d29f1cdfb8e61ca091a9fa5e63acb3b5db0551`  
		Last Modified: Wed, 19 Aug 2020 22:15:02 GMT  
		Size: 55.0 MB (55006878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:34fc3a3495a7ff8a15d4b459a63c6483ecd1efd3fff60609ffaf202727807e52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.2 MB (109161545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701a1f5cdfc6c53cefb236bd347a775688a9c77695119fd6768d8ed74863c6ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:10 GMT
ADD file:d2bdf56089aa739c01f4fea190a17051fbcd45e31fa5ba26d466921d4b528a06 in / 
# Wed, 19 Aug 2020 21:16:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:16:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:49 GMT
CMD ["/bin/bash"]
# Thu, 20 Aug 2020 00:32:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:33:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 20 Aug 2020 00:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd233d33322880c9108ff9d4a2836417f422f1f76cea04cbce12861b48e4ec0a`  
		Last Modified: Mon, 17 Aug 2020 15:54:01 GMT  
		Size: 33.5 MB (33521520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948f26d4116ec9c2f8ce7b5d3765e3f977e8e62da7b636f40f1d3d554b6027e3`  
		Last Modified: Wed, 19 Aug 2020 21:19:34 GMT  
		Size: 30.9 KB (30877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2568d3b37f18de7a6f08771049d897ef5d8bdbf2ddba783262fee3d781a2c588`  
		Last Modified: Wed, 19 Aug 2020 21:19:33 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271de21485d292cc9b05d3b055184c64751e0cf915de5be7c595ef973f80d104`  
		Last Modified: Wed, 19 Aug 2020 21:19:33 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e242cd3731e0ee7c6107fbde83668bf7dbbc2f329278aa64548b8b6e69ca1e`  
		Last Modified: Thu, 20 Aug 2020 01:06:16 GMT  
		Size: 7.8 MB (7816668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0357a04a0eaa3f73a4e0de3317b10e7b6ee2cff741c22e8b4cd78cab3c8d0b77`  
		Last Modified: Thu, 20 Aug 2020 01:06:15 GMT  
		Size: 4.4 MB (4446779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4acf10fdc3db810bf8d904b3a9bf00377f86aa5ac5f0f7a7705f15edc031154`  
		Last Modified: Thu, 20 Aug 2020 01:06:41 GMT  
		Size: 63.3 MB (63344665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5808829be7d01ad0f2596c4e115dda401bc43db292d2a09b72a53908f620d24e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.6 MB (93576431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:413cc585601e8a328c7e1b6adadae1fbc9aee927dc029488649e221dea087810`
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
# Wed, 19 Aug 2020 21:49:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0bd2cd60be73e971313a4fb761143ad4f8e334d3e38e3e36d0a97e556451c785`  
		Last Modified: Wed, 19 Aug 2020 21:54:19 GMT  
		Size: 54.8 MB (54839776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
