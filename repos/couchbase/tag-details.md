<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.4`](#couchbase604)
-	[`couchbase:6.6.0`](#couchbase660)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.4`](#couchbaseenterprise-604)
-	[`couchbase:enterprise-6.6.0`](#couchbaseenterprise-660)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.4`

```console
$ docker pull couchbase@sha256:6aad68234597263847c8204480b8feb16e3a1d5a98bd4c4c039a290c248dc961
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:9b8c2e936d8af11987cbba26bb9d6788b1ef267a0354b665548415716cd70246
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **480.6 MB (480600116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a35fc45655908f0a8c143b08ffa6935f7c87515bdc00fac5f6b96735ebbc4ed2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:58:57 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:58:59 GMT
ARG CB_VERSION=6.0.4
# Wed, 16 Sep 2020 23:59:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Wed, 16 Sep 2020 23:59:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:59:02 GMT
ARG CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf
# Wed, 16 Sep 2020 23:59:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:59:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:59:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:59:50 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:59:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:59:51 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:59:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:59:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:59:53 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:59:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:59:53 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:59:53 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:59:53 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bc3e8d92877ea34000453809f623ed10d9f69250e6a05b6fa905a78ff3f4e`  
		Last Modified: Thu, 17 Sep 2020 00:02:22 GMT  
		Size: 14.3 MB (14284822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ab0b19a5bab4ebed5833da56c84029e3a3434a413e32fdfb116f2c71444e8`  
		Last Modified: Thu, 17 Sep 2020 00:02:18 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed917ca5114055c393f0687e29a4e2d6a7c4518db60d97600d97d7fdc5560b9`  
		Last Modified: Thu, 17 Sep 2020 00:03:03 GMT  
		Size: 421.7 MB (421698137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272d30e9dcd3511fd9131d051fa2cb554167291df4294e97f8074aafe3f67a8`  
		Last Modified: Thu, 17 Sep 2020 00:02:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6b750ced254ab0d0dd97451105b931667e71e34e6243764969573e16260740`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923730a2c7a0a8894ac960bcfd2ad49a0f988431c3605b793a5eac873c62b03c`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26c9ef544078e093d6eb43efc05702985c17cd4db48c8baf94bc223b0757592`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bedf485b8f9fecc62288c16123f6bbe7bda448724dd6c8cb9fd88d3a208773`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 120.6 KB (120598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeb2b4ef271ce3199a3c5b16750b3b48569ecac0a6dfff91f97c96cae2fe11`  
		Last Modified: Thu, 17 Sep 2020 00:02:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.0`

```console
$ docker pull couchbase@sha256:7b3d5fab2ce0874e3c9c592fef5b23e9261761771544777d58da7dd5a5d2a8a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:33a751f77c73af46530e28d23b15a1610df2076ce294698792b467e1a2a1173a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 MB (541762006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0266a58ce0e676e3aab9b96f83a06875ebe3c80de6e75c84d74d605b3fa6252`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:56:33 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Wed, 16 Sep 2020 23:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:57:30 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:57:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:57:33 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:57:33 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:57:33 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:57:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8749ec1c1e66c99f8c42155075d7d208921a2fbaed312f6e617d6c4680ca6309`  
		Last Modified: Thu, 17 Sep 2020 00:00:17 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c14103702b8a956b670448832897668f7443ec26b2095328977319b292f09`  
		Last Modified: Thu, 17 Sep 2020 00:01:16 GMT  
		Size: 491.3 MB (491320019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eba528fabb0e5775adb78a07d1042681331ac5b287eb22d6c7f93626cb60cc`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65d688c797084d4f1e7b558eb0cb4b8fee1714c2374108b7190aacd114cb18`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b159bd9951b4e16aae619e1928df4f2ab52ba7db335b2d476f438844375bd88f`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2e784af48b204685a2ab2072fe714c90517ed7ebbc515e3afb13cf593cbfb`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffc8117c5c55028c9eb93a77d7bbb49c5a8f31927384dde9383ddea26ca32e0`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487384ac1cb40b5b5b3d0bd457fa8bee0dbcd3b83eb395f47592596cb0e5fca`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 118.1 KB (118072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0171f2f8d3d6117b7b9f6fb9d3e98288702d75bf8fef4bfb808b443a9273a1`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:bfee3647e940dd983b0feacb80288c7e40c3a6b635efff28b065c60f0122a07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:e66373bbcea44b2743bea4a2f861e488f634aaf8fd0814311bbc5b2ac102df72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370014427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f72cc9a34f0be11fdfab884af7cdfc680db7ae655f1e9df4f2e891441e263724`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:57:43 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:57:43 GMT
ARG CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e
# Wed, 16 Sep 2020 23:57:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:57:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:58:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:58:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:58:27 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:58:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:58:28 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:58:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:58:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:58:30 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:58:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:58:30 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:58:30 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:58:30 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b12c3b615873ea1de0c6d3ba0734c1de2c779a386353bd8a81c3a0bb4b21dc3`  
		Last Modified: Thu, 17 Sep 2020 00:01:32 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8781ea83c7896fa417e358709ab38079e5c2e9b3dad23c50a3545fd2a0cff18`  
		Last Modified: Thu, 17 Sep 2020 00:02:12 GMT  
		Size: 319.6 MB (319572441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a74dda94e5ae9e93f33dd497eaca52ed84278d1c440ebe39a790fb7403e5d19`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cd67d73a2679bf46584b80874cca2c8a7e15771e58fb5b9cc938f77d748c3c`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a211320e1ef1673c73000c1027450d7af204a88d92571b110f5111778057d`  
		Last Modified: Thu, 17 Sep 2020 00:01:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854c996076819b24ae53e5ad1a0fe6ad50dc47a8125e1f46564b3f4df08093d1`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81f397beb9ed3d4a2c486bd87c92a74e83e883f1092c6297f5c00705912c70f`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effd614f0d556ae32838c4827a8352c68b17e2bfc3902b9c319dcf5a2bcec88d`  
		Last Modified: Thu, 17 Sep 2020 00:01:30 GMT  
		Size: 118.1 KB (118073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a146529fd949db8b976ef8ae508afb882fa89c27b4dc329fec2a6a56444da5`  
		Last Modified: Thu, 17 Sep 2020 00:01:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:bfee3647e940dd983b0feacb80288c7e40c3a6b635efff28b065c60f0122a07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:e66373bbcea44b2743bea4a2f861e488f634aaf8fd0814311bbc5b2ac102df72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370014427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f72cc9a34f0be11fdfab884af7cdfc680db7ae655f1e9df4f2e891441e263724`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:57:43 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:57:43 GMT
ARG CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e
# Wed, 16 Sep 2020 23:57:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:57:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:58:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:58:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:58:27 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:58:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:58:28 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:58:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:58:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:58:30 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:58:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:58:30 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:58:30 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:58:30 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b12c3b615873ea1de0c6d3ba0734c1de2c779a386353bd8a81c3a0bb4b21dc3`  
		Last Modified: Thu, 17 Sep 2020 00:01:32 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8781ea83c7896fa417e358709ab38079e5c2e9b3dad23c50a3545fd2a0cff18`  
		Last Modified: Thu, 17 Sep 2020 00:02:12 GMT  
		Size: 319.6 MB (319572441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a74dda94e5ae9e93f33dd497eaca52ed84278d1c440ebe39a790fb7403e5d19`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cd67d73a2679bf46584b80874cca2c8a7e15771e58fb5b9cc938f77d748c3c`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a211320e1ef1673c73000c1027450d7af204a88d92571b110f5111778057d`  
		Last Modified: Thu, 17 Sep 2020 00:01:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854c996076819b24ae53e5ad1a0fe6ad50dc47a8125e1f46564b3f4df08093d1`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81f397beb9ed3d4a2c486bd87c92a74e83e883f1092c6297f5c00705912c70f`  
		Last Modified: Thu, 17 Sep 2020 00:01:31 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effd614f0d556ae32838c4827a8352c68b17e2bfc3902b9c319dcf5a2bcec88d`  
		Last Modified: Thu, 17 Sep 2020 00:01:30 GMT  
		Size: 118.1 KB (118073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a146529fd949db8b976ef8ae508afb882fa89c27b4dc329fec2a6a56444da5`  
		Last Modified: Thu, 17 Sep 2020 00:01:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:7b3d5fab2ce0874e3c9c592fef5b23e9261761771544777d58da7dd5a5d2a8a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:33a751f77c73af46530e28d23b15a1610df2076ce294698792b467e1a2a1173a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 MB (541762006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0266a58ce0e676e3aab9b96f83a06875ebe3c80de6e75c84d74d605b3fa6252`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:56:33 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Wed, 16 Sep 2020 23:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:57:30 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:57:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:57:33 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:57:33 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:57:33 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:57:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8749ec1c1e66c99f8c42155075d7d208921a2fbaed312f6e617d6c4680ca6309`  
		Last Modified: Thu, 17 Sep 2020 00:00:17 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c14103702b8a956b670448832897668f7443ec26b2095328977319b292f09`  
		Last Modified: Thu, 17 Sep 2020 00:01:16 GMT  
		Size: 491.3 MB (491320019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eba528fabb0e5775adb78a07d1042681331ac5b287eb22d6c7f93626cb60cc`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65d688c797084d4f1e7b558eb0cb4b8fee1714c2374108b7190aacd114cb18`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b159bd9951b4e16aae619e1928df4f2ab52ba7db335b2d476f438844375bd88f`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2e784af48b204685a2ab2072fe714c90517ed7ebbc515e3afb13cf593cbfb`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffc8117c5c55028c9eb93a77d7bbb49c5a8f31927384dde9383ddea26ca32e0`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487384ac1cb40b5b5b3d0bd457fa8bee0dbcd3b83eb395f47592596cb0e5fca`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 118.1 KB (118072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0171f2f8d3d6117b7b9f6fb9d3e98288702d75bf8fef4bfb808b443a9273a1`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.4`

```console
$ docker pull couchbase@sha256:6aad68234597263847c8204480b8feb16e3a1d5a98bd4c4c039a290c248dc961
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:9b8c2e936d8af11987cbba26bb9d6788b1ef267a0354b665548415716cd70246
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **480.6 MB (480600116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a35fc45655908f0a8c143b08ffa6935f7c87515bdc00fac5f6b96735ebbc4ed2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:58:57 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:58:59 GMT
ARG CB_VERSION=6.0.4
# Wed, 16 Sep 2020 23:59:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Wed, 16 Sep 2020 23:59:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:59:02 GMT
ARG CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf
# Wed, 16 Sep 2020 23:59:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:59:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:59:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:59:50 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:59:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:59:51 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:59:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:59:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:59:53 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:59:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:59:53 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:59:53 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:59:53 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bc3e8d92877ea34000453809f623ed10d9f69250e6a05b6fa905a78ff3f4e`  
		Last Modified: Thu, 17 Sep 2020 00:02:22 GMT  
		Size: 14.3 MB (14284822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ab0b19a5bab4ebed5833da56c84029e3a3434a413e32fdfb116f2c71444e8`  
		Last Modified: Thu, 17 Sep 2020 00:02:18 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed917ca5114055c393f0687e29a4e2d6a7c4518db60d97600d97d7fdc5560b9`  
		Last Modified: Thu, 17 Sep 2020 00:03:03 GMT  
		Size: 421.7 MB (421698137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272d30e9dcd3511fd9131d051fa2cb554167291df4294e97f8074aafe3f67a8`  
		Last Modified: Thu, 17 Sep 2020 00:02:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6b750ced254ab0d0dd97451105b931667e71e34e6243764969573e16260740`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923730a2c7a0a8894ac960bcfd2ad49a0f988431c3605b793a5eac873c62b03c`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26c9ef544078e093d6eb43efc05702985c17cd4db48c8baf94bc223b0757592`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bedf485b8f9fecc62288c16123f6bbe7bda448724dd6c8cb9fd88d3a208773`  
		Last Modified: Thu, 17 Sep 2020 00:02:17 GMT  
		Size: 120.6 KB (120598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeb2b4ef271ce3199a3c5b16750b3b48569ecac0a6dfff91f97c96cae2fe11`  
		Last Modified: Thu, 17 Sep 2020 00:02:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.0`

```console
$ docker pull couchbase@sha256:7b3d5fab2ce0874e3c9c592fef5b23e9261761771544777d58da7dd5a5d2a8a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:33a751f77c73af46530e28d23b15a1610df2076ce294698792b467e1a2a1173a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 MB (541762006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0266a58ce0e676e3aab9b96f83a06875ebe3c80de6e75c84d74d605b3fa6252`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:56:33 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Wed, 16 Sep 2020 23:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:57:30 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:57:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:57:33 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:57:33 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:57:33 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:57:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8749ec1c1e66c99f8c42155075d7d208921a2fbaed312f6e617d6c4680ca6309`  
		Last Modified: Thu, 17 Sep 2020 00:00:17 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c14103702b8a956b670448832897668f7443ec26b2095328977319b292f09`  
		Last Modified: Thu, 17 Sep 2020 00:01:16 GMT  
		Size: 491.3 MB (491320019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eba528fabb0e5775adb78a07d1042681331ac5b287eb22d6c7f93626cb60cc`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65d688c797084d4f1e7b558eb0cb4b8fee1714c2374108b7190aacd114cb18`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b159bd9951b4e16aae619e1928df4f2ab52ba7db335b2d476f438844375bd88f`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2e784af48b204685a2ab2072fe714c90517ed7ebbc515e3afb13cf593cbfb`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffc8117c5c55028c9eb93a77d7bbb49c5a8f31927384dde9383ddea26ca32e0`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487384ac1cb40b5b5b3d0bd457fa8bee0dbcd3b83eb395f47592596cb0e5fca`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 118.1 KB (118072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0171f2f8d3d6117b7b9f6fb9d3e98288702d75bf8fef4bfb808b443a9273a1`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:7b3d5fab2ce0874e3c9c592fef5b23e9261761771544777d58da7dd5a5d2a8a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:33a751f77c73af46530e28d23b15a1610df2076ce294698792b467e1a2a1173a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 MB (541762006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0266a58ce0e676e3aab9b96f83a06875ebe3c80de6e75c84d74d605b3fa6252`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:56:33 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Wed, 16 Sep 2020 23:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:57:30 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:57:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:57:33 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:57:33 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:57:33 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:57:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8749ec1c1e66c99f8c42155075d7d208921a2fbaed312f6e617d6c4680ca6309`  
		Last Modified: Thu, 17 Sep 2020 00:00:17 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c14103702b8a956b670448832897668f7443ec26b2095328977319b292f09`  
		Last Modified: Thu, 17 Sep 2020 00:01:16 GMT  
		Size: 491.3 MB (491320019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eba528fabb0e5775adb78a07d1042681331ac5b287eb22d6c7f93626cb60cc`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65d688c797084d4f1e7b558eb0cb4b8fee1714c2374108b7190aacd114cb18`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b159bd9951b4e16aae619e1928df4f2ab52ba7db335b2d476f438844375bd88f`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2e784af48b204685a2ab2072fe714c90517ed7ebbc515e3afb13cf593cbfb`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffc8117c5c55028c9eb93a77d7bbb49c5a8f31927384dde9383ddea26ca32e0`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487384ac1cb40b5b5b3d0bd457fa8bee0dbcd3b83eb395f47592596cb0e5fca`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 118.1 KB (118072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0171f2f8d3d6117b7b9f6fb9d3e98288702d75bf8fef4bfb808b443a9273a1`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
