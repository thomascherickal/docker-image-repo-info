<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.5`](#couchbase605)
-	[`couchbase:6.6.4`](#couchbase664)
-	[`couchbase:7.0.3`](#couchbase703)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.2`](#couchbasecommunity-702)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.5`](#couchbaseenterprise-605)
-	[`couchbase:enterprise-6.6.4`](#couchbaseenterprise-664)
-	[`couchbase:enterprise-7.0.3`](#couchbaseenterprise-703)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.5`

```console
$ docker pull couchbase@sha256:f7367d3afa61523b212b188b2180489014d9f2fda592d5423db7721c64d8c11f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:192ee4cbb0554bdc6fd470dba43e72b21a3fdc31c0d1b803f268b5ac01ede908
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466121342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe105794e8b009d8881de173968dd3e0beaa0cb7b92823d6d0923fca3089adb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:46:10 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 01 Oct 2021 02:48:17 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:48:18 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_VERSION=6.0.5
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Fri, 01 Oct 2021 02:48:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 01 Oct 2021 02:48:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 01 Oct 2021 02:49:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:49:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 01 Oct 2021 02:49:21 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 01 Oct 2021 02:49:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 01 Oct 2021 02:49:22 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 01 Oct 2021 02:49:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 01 Oct 2021 02:49:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 01 Oct 2021 02:49:24 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 01 Oct 2021 02:49:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Oct 2021 02:49:25 GMT
CMD ["couchbase-server"]
# Fri, 01 Oct 2021 02:49:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 01 Oct 2021 02:49:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7533055455fc3b7edab1b7d1a254e5048632115db3ed069e464a9f70b46f9701`  
		Last Modified: Fri, 01 Oct 2021 02:54:27 GMT  
		Size: 15.9 MB (15923249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1101292f94db4a63208276d651c0e7aefbf97c3c251c37fd3ed1589de11b8256`  
		Last Modified: Fri, 01 Oct 2021 02:54:23 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5158df84771ac1ab261a6fc30d9f422d4096eca3399d47d1bd563a998fa8929`  
		Last Modified: Fri, 01 Oct 2021 02:54:22 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48c9e9bde3e55d56cbbc3043140d87c593e1862ac0ef784e25c525f90fb3867`  
		Last Modified: Fri, 01 Oct 2021 02:55:02 GMT  
		Size: 423.4 MB (423362973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0e391c7a9a7cc6b458c7e5bee36ffe1abb7751253533e1d7fb7321c07cbb1a`  
		Last Modified: Fri, 01 Oct 2021 02:54:22 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5547d6ef3793148e40087c50a166c4789e06fd3bc0e804caa204fe87e2b8363`  
		Last Modified: Fri, 01 Oct 2021 02:54:22 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc4ef267815398c6a0295a86023660d9edaa17a43b72fb485b20b834ed9f395`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2e6c182c0b9532500fd2b68eff31064940290cccbdfcaca3cfdb1ec9fe7809`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8243cd47a1656c57e01fb7d79bd1472b3b9e82f0b8a60ffdef25f2d8b00b4b26`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c87f7b248d9297630c286186f37bb21b3139a825473a75a09b7c88438e429fd`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 125.6 KB (125557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eb17d4605e78b6b469806e8abcfc577253ea890fe8859206c383f57fbb6ccf`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.4`

```console
$ docker pull couchbase@sha256:742a3a56b938762755b8a6be4b22bd3e3f3be62e337187e6729788690cdc9816
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.4` - linux; amd64

```console
$ docker pull couchbase@sha256:8c532b453a34222940ac42ca88873037ac402f64b6e7eb0a91b474226adfabc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561397822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee9cd50ae8946ba8ebe8e2ede1839b6dc4275050d5855dfc438c95ec527ed19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 14 Dec 2021 18:20:05 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:21:37 GMT
ARG CB_VERSION=6.6.4
# Tue, 14 Dec 2021 18:21:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4
# Tue, 14 Dec 2021 18:21:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb
# Tue, 14 Dec 2021 18:21:38 GMT
ARG CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db
# Tue, 14 Dec 2021 18:21:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 14 Dec 2021 18:21:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 14 Dec 2021 18:22:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:22:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 14 Dec 2021 18:22:37 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 14 Dec 2021 18:22:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 14 Dec 2021 18:22:38 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 14 Dec 2021 18:22:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 14 Dec 2021 18:22:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             apt-get update;             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get purge -y chrpath;             apt-get autoremove;             apt-get clean;         fi
# Tue, 14 Dec 2021 18:22:45 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 14 Dec 2021 18:22:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Dec 2021 18:22:46 GMT
CMD ["couchbase-server"]
# Tue, 14 Dec 2021 18:22:46 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 14 Dec 2021 18:22:46 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7121d42a6972f1cbcce5d40298238b9d7b9f3322ae0dc2998efb6c7e832913`  
		Last Modified: Tue, 14 Dec 2021 18:23:23 GMT  
		Size: 6.3 MB (6252763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ae2706cce78cc381f693caf3dad1e366edbd9b0bdb6ab2283cb2fd7e6e17c`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4583df08983d2785848cc508ec47cf0f64e902a30797ca7ddfe73744411aa`  
		Last Modified: Tue, 14 Dec 2021 18:25:36 GMT  
		Size: 503.0 MB (502991734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec819eb023f8b5f1052a45426a64d30de1c5d2f7494d7c6dfc9a0859e879a4b`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5e493d219800f51a412e514f454fc314ae22db88c45d571806cd9febbfc3c2`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b0b11d9eeb8db83e86e98aefb3164f62bbd489456ee750b5594f8c1b42f6`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21e7cb4b83b7a64baf17e9153f5bbbbe15087ff8976138f742952ded53e973a`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d21a5daa1dc524b59c9c2019f3c6521e6ee59785f6464faa8dae410f901880`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cf888488427006085e81f6e1e97e76de2f1ea36e832770bd5b2c8d76cb2398`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 23.6 MB (23581843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8cbd2a908b899eeb9d8cd145fffdbc4cc933fe2628fa6aacd34c1d68f7c4e7`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.3`

```console
$ docker pull couchbase@sha256:bbed75ede6d1fa0ed395fa46659ba8eada36c59535043051d8ef47ed3d5113b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:f319e2e60eb1231197546238dfdfccaf7d98540fb62d0b716c400ba507dce28a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.7 MB (676707538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:263093b8c6566e677359373ca4825c7cf5f83aaa4789d846986fdb8d1d79c0d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 14 Dec 2021 18:20:05 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_VERSION=7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c
# Tue, 14 Dec 2021 18:20:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 14 Dec 2021 18:20:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 14 Dec 2021 18:21:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:21:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 14 Dec 2021 18:21:14 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 14 Dec 2021 18:21:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 14 Dec 2021 18:21:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 14 Dec 2021 18:21:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 14 Dec 2021 18:21:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             apt-get update;             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get purge -y chrpath;             apt-get autoremove;             apt-get clean;         fi
# Tue, 14 Dec 2021 18:21:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 14 Dec 2021 18:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Dec 2021 18:21:23 GMT
CMD ["couchbase-server"]
# Tue, 14 Dec 2021 18:21:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 14 Dec 2021 18:21:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7121d42a6972f1cbcce5d40298238b9d7b9f3322ae0dc2998efb6c7e832913`  
		Last Modified: Tue, 14 Dec 2021 18:23:23 GMT  
		Size: 6.3 MB (6252763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dca40ea6b0f35b34a260b3201f68e776570a0864f41cea6a33404e21fcbe20`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8b28333f514f833e264948ff359ae8dd3a2c8dacad7956d163b25dbecd5cd`  
		Last Modified: Tue, 14 Dec 2021 18:24:24 GMT  
		Size: 618.3 MB (618297736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0eb674025044d8d6914d9418ebff99111bd07908c909549c3f4c868ce74984`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ec5ac06458ac7d7cd7bb49c2705a53f448f10f5cecf5cc9b4c33cda0cbd13`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e050d2e5f7be287022a8f70b6633188c6c4388588a56f03790deb99e094194`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525c0205c5d17582b72d9d489411f5862afa2de165f8095c4aeab80ad1c562b`  
		Last Modified: Tue, 14 Dec 2021 18:23:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7052545fe7c7e0fc79c30dec1074f6a2a6fccb5223bbc681a9d3b44e3acd8dd`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646896311425b412d73a2437efa3f296df91a7f53d10a4a40b2b47c239f7fa07`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 23.6 MB (23585553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44377da25a87afb3e79d307250380fb0aab61fea24b8fcc25d70f02d207c016c`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:f402d64919aaa3456913c503f2aa55e2f337776329e0cdd7e48e4eec4121be9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:45604b674bf5b0ae801b518454aa6086c6075a2a923060f05db894a113476296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429028273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b879a3ddad222da8c00fa3ef26ba4d44ad3f9d5eca221be8e9e188255abc6bd2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 16 Oct 2021 01:57:08 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 16 Oct 2021 01:57:09 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 16 Oct 2021 01:57:09 GMT
ARG CB_VERSION=7.0.2
# Sat, 16 Oct 2021 01:57:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 16 Oct 2021 01:58:26 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 16 Oct 2021 01:58:26 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 16 Oct 2021 01:58:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 16 Oct 2021 01:58:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 16 Oct 2021 01:59:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 16 Oct 2021 01:59:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 16 Oct 2021 01:59:14 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 16 Oct 2021 01:59:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 16 Oct 2021 01:59:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:59:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 16 Oct 2021 01:59:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 16 Oct 2021 01:59:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 16 Oct 2021 01:59:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 01:59:17 GMT
CMD ["couchbase-server"]
# Sat, 16 Oct 2021 01:59:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 16 Oct 2021 01:59:17 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e0b832017c5b057450b3c05d02cd15d9687606589e0446fa6329ae65e7f32`  
		Last Modified: Sat, 16 Oct 2021 02:00:56 GMT  
		Size: 6.3 MB (6265546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6682df4a3ff50d93156aa026b6e11d7d533b0cbdf3ca9603a87c4d00d3b6041b`  
		Last Modified: Sat, 16 Oct 2021 02:00:53 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aff14a2108d1c8af97820910830806940d3da9305a9ea3c5805d21699a81d74`  
		Last Modified: Sat, 16 Oct 2021 02:02:16 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02bccf83ffe78f7c2cbb1895ab812fcd7d8000088b04e99f44de33942cc18c0`  
		Last Modified: Sat, 16 Oct 2021 02:03:02 GMT  
		Size: 394.1 MB (394061631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3804e30d842d14a3973ea9bb6c61050d3bdda76e096aae21fbadf37ec59b6dc0`  
		Last Modified: Sat, 16 Oct 2021 02:02:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f827773d002bd1f23ea096f6f51b7972e69d29321817c266b8808979f349a5`  
		Last Modified: Sat, 16 Oct 2021 02:02:16 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbf9c09f41b2ca05c10f145b15cee3f720bc744ae87927e34ab1cec65d45410`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c32b7911fb70167e68716a8fcc063fd36d7adb6c7042cdfb1050074817bf12a`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2baa9d0ce0b6d64ef85b6581beb55cf5cbe37f110fafc29b5cc12b2f7129e2b`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b548404873a0581b2c88ffee8020ca1db39d8ef450915ac047025cf59fe69eb6`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 129.5 KB (129508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a96376676eaa559484c9287f9ef8943fefd716a8a3204a40a8e2315fbd3d9a`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:aa1d1ecb1c9acf92eb9dba4fd5a3be27732873489ce12f06dcb7505bdad5bd38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:f37cccde0714e86e0a3cd0a0c97c4a0a3cf1b03b96889fa8fb0b884e08e69e2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354217687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892ead5439a2e0678c39beac392508fc6ed5db3913320189829c30b1dca40bac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:46:10 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 01 Oct 2021 02:46:44 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:46:45 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 01 Oct 2021 02:46:45 GMT
ARG CB_VERSION=6.6.0
# Fri, 01 Oct 2021 02:46:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 01 Oct 2021 02:46:46 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Fri, 01 Oct 2021 02:46:46 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Fri, 01 Oct 2021 02:46:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 01 Oct 2021 02:46:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 01 Oct 2021 02:47:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:47:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 01 Oct 2021 02:47:37 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 01 Oct 2021 02:47:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 01 Oct 2021 02:47:38 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 01 Oct 2021 02:47:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 01 Oct 2021 02:47:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 01 Oct 2021 02:47:39 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 01 Oct 2021 02:47:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Oct 2021 02:47:40 GMT
CMD ["couchbase-server"]
# Fri, 01 Oct 2021 02:47:40 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 01 Oct 2021 02:47:40 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7178ada3bd73aa22d37d77aa136877737ee4011b10f2b5491bcf219a3a19748c`  
		Last Modified: Fri, 01 Oct 2021 02:53:37 GMT  
		Size: 7.4 MB (7371489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e73dd26d67d7da2e2befe37ab77651e48cd18cf43ed4c858263d9470517a15`  
		Last Modified: Fri, 01 Oct 2021 02:53:34 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c411f8d03c30662fcf56518f0a72d017871e6f25a52a2772060a391c86282ae`  
		Last Modified: Fri, 01 Oct 2021 02:53:34 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f502a2583d022678ba882b83325f622633840be055d51ec59aa773ee12bb67c8`  
		Last Modified: Fri, 01 Oct 2021 02:54:12 GMT  
		Size: 320.0 MB (320018444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a38d674cffc30e7883414b19c151e05c98c969be1e26986fc4f0f9af59398f`  
		Last Modified: Fri, 01 Oct 2021 02:53:34 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd1ce8cfac06dd358c19fb4ad8c4f0d3243934efe2a699612249f0ff92cc540`  
		Last Modified: Fri, 01 Oct 2021 02:53:34 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65037115b1fb0270bd3facc9fbf4b72533b46bc766a7d324d37326e418787ee7`  
		Last Modified: Fri, 01 Oct 2021 02:53:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b2f5d17a30c0613666f64eee4029e7c89c43c1c9615747c909f01b1289272e`  
		Last Modified: Fri, 01 Oct 2021 02:53:31 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f75fd1fb20db52b01d1d77c7ef924a48dfd6b0c5549505626ed49af5cc707e`  
		Last Modified: Fri, 01 Oct 2021 02:53:32 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbffe15c5f9ca3a1da255be0641f813436e87681652d18b939e821d4aa5dcacf`  
		Last Modified: Fri, 01 Oct 2021 02:53:32 GMT  
		Size: 118.2 KB (118189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08208822bdae9d3fd0a0a7e9e36574647c9e2048111154fc33f88a3c414c2ef2`  
		Last Modified: Fri, 01 Oct 2021 02:53:31 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:f402d64919aaa3456913c503f2aa55e2f337776329e0cdd7e48e4eec4121be9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:45604b674bf5b0ae801b518454aa6086c6075a2a923060f05db894a113476296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429028273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b879a3ddad222da8c00fa3ef26ba4d44ad3f9d5eca221be8e9e188255abc6bd2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 16 Oct 2021 01:57:08 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 16 Oct 2021 01:57:09 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 16 Oct 2021 01:57:09 GMT
ARG CB_VERSION=7.0.2
# Sat, 16 Oct 2021 01:57:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 16 Oct 2021 01:58:26 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 16 Oct 2021 01:58:26 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 16 Oct 2021 01:58:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 16 Oct 2021 01:58:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 16 Oct 2021 01:59:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 16 Oct 2021 01:59:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 16 Oct 2021 01:59:14 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 16 Oct 2021 01:59:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 16 Oct 2021 01:59:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 16 Oct 2021 01:59:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 16 Oct 2021 01:59:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 16 Oct 2021 01:59:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 16 Oct 2021 01:59:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 01:59:17 GMT
CMD ["couchbase-server"]
# Sat, 16 Oct 2021 01:59:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 16 Oct 2021 01:59:17 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e0b832017c5b057450b3c05d02cd15d9687606589e0446fa6329ae65e7f32`  
		Last Modified: Sat, 16 Oct 2021 02:00:56 GMT  
		Size: 6.3 MB (6265546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6682df4a3ff50d93156aa026b6e11d7d533b0cbdf3ca9603a87c4d00d3b6041b`  
		Last Modified: Sat, 16 Oct 2021 02:00:53 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aff14a2108d1c8af97820910830806940d3da9305a9ea3c5805d21699a81d74`  
		Last Modified: Sat, 16 Oct 2021 02:02:16 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02bccf83ffe78f7c2cbb1895ab812fcd7d8000088b04e99f44de33942cc18c0`  
		Last Modified: Sat, 16 Oct 2021 02:03:02 GMT  
		Size: 394.1 MB (394061631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3804e30d842d14a3973ea9bb6c61050d3bdda76e096aae21fbadf37ec59b6dc0`  
		Last Modified: Sat, 16 Oct 2021 02:02:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f827773d002bd1f23ea096f6f51b7972e69d29321817c266b8808979f349a5`  
		Last Modified: Sat, 16 Oct 2021 02:02:16 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbf9c09f41b2ca05c10f145b15cee3f720bc744ae87927e34ab1cec65d45410`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c32b7911fb70167e68716a8fcc063fd36d7adb6c7042cdfb1050074817bf12a`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2baa9d0ce0b6d64ef85b6581beb55cf5cbe37f110fafc29b5cc12b2f7129e2b`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b548404873a0581b2c88ffee8020ca1db39d8ef450915ac047025cf59fe69eb6`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 129.5 KB (129508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a96376676eaa559484c9287f9ef8943fefd716a8a3204a40a8e2315fbd3d9a`  
		Last Modified: Sat, 16 Oct 2021 02:02:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:bbed75ede6d1fa0ed395fa46659ba8eada36c59535043051d8ef47ed3d5113b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:f319e2e60eb1231197546238dfdfccaf7d98540fb62d0b716c400ba507dce28a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.7 MB (676707538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:263093b8c6566e677359373ca4825c7cf5f83aaa4789d846986fdb8d1d79c0d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 14 Dec 2021 18:20:05 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_VERSION=7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c
# Tue, 14 Dec 2021 18:20:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 14 Dec 2021 18:20:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 14 Dec 2021 18:21:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:21:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 14 Dec 2021 18:21:14 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 14 Dec 2021 18:21:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 14 Dec 2021 18:21:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 14 Dec 2021 18:21:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 14 Dec 2021 18:21:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             apt-get update;             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get purge -y chrpath;             apt-get autoremove;             apt-get clean;         fi
# Tue, 14 Dec 2021 18:21:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 14 Dec 2021 18:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Dec 2021 18:21:23 GMT
CMD ["couchbase-server"]
# Tue, 14 Dec 2021 18:21:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 14 Dec 2021 18:21:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7121d42a6972f1cbcce5d40298238b9d7b9f3322ae0dc2998efb6c7e832913`  
		Last Modified: Tue, 14 Dec 2021 18:23:23 GMT  
		Size: 6.3 MB (6252763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dca40ea6b0f35b34a260b3201f68e776570a0864f41cea6a33404e21fcbe20`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8b28333f514f833e264948ff359ae8dd3a2c8dacad7956d163b25dbecd5cd`  
		Last Modified: Tue, 14 Dec 2021 18:24:24 GMT  
		Size: 618.3 MB (618297736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0eb674025044d8d6914d9418ebff99111bd07908c909549c3f4c868ce74984`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ec5ac06458ac7d7cd7bb49c2705a53f448f10f5cecf5cc9b4c33cda0cbd13`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e050d2e5f7be287022a8f70b6633188c6c4388588a56f03790deb99e094194`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525c0205c5d17582b72d9d489411f5862afa2de165f8095c4aeab80ad1c562b`  
		Last Modified: Tue, 14 Dec 2021 18:23:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7052545fe7c7e0fc79c30dec1074f6a2a6fccb5223bbc681a9d3b44e3acd8dd`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646896311425b412d73a2437efa3f296df91a7f53d10a4a40b2b47c239f7fa07`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 23.6 MB (23585553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44377da25a87afb3e79d307250380fb0aab61fea24b8fcc25d70f02d207c016c`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:f7367d3afa61523b212b188b2180489014d9f2fda592d5423db7721c64d8c11f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:192ee4cbb0554bdc6fd470dba43e72b21a3fdc31c0d1b803f268b5ac01ede908
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466121342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe105794e8b009d8881de173968dd3e0beaa0cb7b92823d6d0923fca3089adb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:46:10 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 01 Oct 2021 02:48:17 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:48:18 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_VERSION=6.0.5
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Fri, 01 Oct 2021 02:48:19 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Fri, 01 Oct 2021 02:48:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 01 Oct 2021 02:48:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 01 Oct 2021 02:49:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:49:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 01 Oct 2021 02:49:21 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 01 Oct 2021 02:49:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 01 Oct 2021 02:49:22 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 01 Oct 2021 02:49:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 01 Oct 2021 02:49:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 01 Oct 2021 02:49:24 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 01 Oct 2021 02:49:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Oct 2021 02:49:25 GMT
CMD ["couchbase-server"]
# Fri, 01 Oct 2021 02:49:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 01 Oct 2021 02:49:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7533055455fc3b7edab1b7d1a254e5048632115db3ed069e464a9f70b46f9701`  
		Last Modified: Fri, 01 Oct 2021 02:54:27 GMT  
		Size: 15.9 MB (15923249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1101292f94db4a63208276d651c0e7aefbf97c3c251c37fd3ed1589de11b8256`  
		Last Modified: Fri, 01 Oct 2021 02:54:23 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5158df84771ac1ab261a6fc30d9f422d4096eca3399d47d1bd563a998fa8929`  
		Last Modified: Fri, 01 Oct 2021 02:54:22 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48c9e9bde3e55d56cbbc3043140d87c593e1862ac0ef784e25c525f90fb3867`  
		Last Modified: Fri, 01 Oct 2021 02:55:02 GMT  
		Size: 423.4 MB (423362973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0e391c7a9a7cc6b458c7e5bee36ffe1abb7751253533e1d7fb7321c07cbb1a`  
		Last Modified: Fri, 01 Oct 2021 02:54:22 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5547d6ef3793148e40087c50a166c4789e06fd3bc0e804caa204fe87e2b8363`  
		Last Modified: Fri, 01 Oct 2021 02:54:22 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc4ef267815398c6a0295a86023660d9edaa17a43b72fb485b20b834ed9f395`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2e6c182c0b9532500fd2b68eff31064940290cccbdfcaca3cfdb1ec9fe7809`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8243cd47a1656c57e01fb7d79bd1472b3b9e82f0b8a60ffdef25f2d8b00b4b26`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c87f7b248d9297630c286186f37bb21b3139a825473a75a09b7c88438e429fd`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 125.6 KB (125557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eb17d4605e78b6b469806e8abcfc577253ea890fe8859206c383f57fbb6ccf`  
		Last Modified: Fri, 01 Oct 2021 02:54:20 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.4`

```console
$ docker pull couchbase@sha256:742a3a56b938762755b8a6be4b22bd3e3f3be62e337187e6729788690cdc9816
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.4` - linux; amd64

```console
$ docker pull couchbase@sha256:8c532b453a34222940ac42ca88873037ac402f64b6e7eb0a91b474226adfabc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561397822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee9cd50ae8946ba8ebe8e2ede1839b6dc4275050d5855dfc438c95ec527ed19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 14 Dec 2021 18:20:05 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:21:37 GMT
ARG CB_VERSION=6.6.4
# Tue, 14 Dec 2021 18:21:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4
# Tue, 14 Dec 2021 18:21:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb
# Tue, 14 Dec 2021 18:21:38 GMT
ARG CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db
# Tue, 14 Dec 2021 18:21:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 14 Dec 2021 18:21:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 14 Dec 2021 18:22:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:22:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 14 Dec 2021 18:22:37 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 14 Dec 2021 18:22:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 14 Dec 2021 18:22:38 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 14 Dec 2021 18:22:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 14 Dec 2021 18:22:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.4 CB_SHA256=97cb0aec5a4f7e3d2c3e2017546ac0adb41478c6e5bc1dcefd06cc9f5926f6db CB_VERSION=6.6.4
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             apt-get update;             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get purge -y chrpath;             apt-get autoremove;             apt-get clean;         fi
# Tue, 14 Dec 2021 18:22:45 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 14 Dec 2021 18:22:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Dec 2021 18:22:46 GMT
CMD ["couchbase-server"]
# Tue, 14 Dec 2021 18:22:46 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 14 Dec 2021 18:22:46 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7121d42a6972f1cbcce5d40298238b9d7b9f3322ae0dc2998efb6c7e832913`  
		Last Modified: Tue, 14 Dec 2021 18:23:23 GMT  
		Size: 6.3 MB (6252763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ae2706cce78cc381f693caf3dad1e366edbd9b0bdb6ab2283cb2fd7e6e17c`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4583df08983d2785848cc508ec47cf0f64e902a30797ca7ddfe73744411aa`  
		Last Modified: Tue, 14 Dec 2021 18:25:36 GMT  
		Size: 503.0 MB (502991734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec819eb023f8b5f1052a45426a64d30de1c5d2f7494d7c6dfc9a0859e879a4b`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5e493d219800f51a412e514f454fc314ae22db88c45d571806cd9febbfc3c2`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b0b11d9eeb8db83e86e98aefb3164f62bbd489456ee750b5594f8c1b42f6`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21e7cb4b83b7a64baf17e9153f5bbbbe15087ff8976138f742952ded53e973a`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d21a5daa1dc524b59c9c2019f3c6521e6ee59785f6464faa8dae410f901880`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cf888488427006085e81f6e1e97e76de2f1ea36e832770bd5b2c8d76cb2398`  
		Last Modified: Tue, 14 Dec 2021 18:24:45 GMT  
		Size: 23.6 MB (23581843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8cbd2a908b899eeb9d8cd145fffdbc4cc933fe2628fa6aacd34c1d68f7c4e7`  
		Last Modified: Tue, 14 Dec 2021 18:24:43 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.3`

```console
$ docker pull couchbase@sha256:bbed75ede6d1fa0ed395fa46659ba8eada36c59535043051d8ef47ed3d5113b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:f319e2e60eb1231197546238dfdfccaf7d98540fb62d0b716c400ba507dce28a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.7 MB (676707538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:263093b8c6566e677359373ca4825c7cf5f83aaa4789d846986fdb8d1d79c0d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 14 Dec 2021 18:20:05 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_VERSION=7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c
# Tue, 14 Dec 2021 18:20:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 14 Dec 2021 18:20:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 14 Dec 2021 18:21:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:21:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 14 Dec 2021 18:21:14 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 14 Dec 2021 18:21:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 14 Dec 2021 18:21:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 14 Dec 2021 18:21:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 14 Dec 2021 18:21:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             apt-get update;             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get purge -y chrpath;             apt-get autoremove;             apt-get clean;         fi
# Tue, 14 Dec 2021 18:21:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 14 Dec 2021 18:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Dec 2021 18:21:23 GMT
CMD ["couchbase-server"]
# Tue, 14 Dec 2021 18:21:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 14 Dec 2021 18:21:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7121d42a6972f1cbcce5d40298238b9d7b9f3322ae0dc2998efb6c7e832913`  
		Last Modified: Tue, 14 Dec 2021 18:23:23 GMT  
		Size: 6.3 MB (6252763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dca40ea6b0f35b34a260b3201f68e776570a0864f41cea6a33404e21fcbe20`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8b28333f514f833e264948ff359ae8dd3a2c8dacad7956d163b25dbecd5cd`  
		Last Modified: Tue, 14 Dec 2021 18:24:24 GMT  
		Size: 618.3 MB (618297736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0eb674025044d8d6914d9418ebff99111bd07908c909549c3f4c868ce74984`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ec5ac06458ac7d7cd7bb49c2705a53f448f10f5cecf5cc9b4c33cda0cbd13`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e050d2e5f7be287022a8f70b6633188c6c4388588a56f03790deb99e094194`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525c0205c5d17582b72d9d489411f5862afa2de165f8095c4aeab80ad1c562b`  
		Last Modified: Tue, 14 Dec 2021 18:23:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7052545fe7c7e0fc79c30dec1074f6a2a6fccb5223bbc681a9d3b44e3acd8dd`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646896311425b412d73a2437efa3f296df91a7f53d10a4a40b2b47c239f7fa07`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 23.6 MB (23585553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44377da25a87afb3e79d307250380fb0aab61fea24b8fcc25d70f02d207c016c`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:bbed75ede6d1fa0ed395fa46659ba8eada36c59535043051d8ef47ed3d5113b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:f319e2e60eb1231197546238dfdfccaf7d98540fb62d0b716c400ba507dce28a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.7 MB (676707538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:263093b8c6566e677359373ca4825c7cf5f83aaa4789d846986fdb8d1d79c0d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:56:48 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 14 Dec 2021 18:20:05 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_VERSION=7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb
# Tue, 14 Dec 2021 18:20:05 GMT
ARG CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c
# Tue, 14 Dec 2021 18:20:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 14 Dec 2021 18:20:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 14 Dec 2021 18:21:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 14 Dec 2021 18:21:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 14 Dec 2021 18:21:14 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 14 Dec 2021 18:21:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 14 Dec 2021 18:21:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 14 Dec 2021 18:21:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 14 Dec 2021 18:21:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3 CB_SHA256=efacf9923a7203771fc342ec010d1baf9325c01f284b22c703b10e5dc9b38d2c CB_VERSION=7.0.3
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             apt-get update;             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get purge -y chrpath;             apt-get autoremove;             apt-get clean;         fi
# Tue, 14 Dec 2021 18:21:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 14 Dec 2021 18:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Dec 2021 18:21:23 GMT
CMD ["couchbase-server"]
# Tue, 14 Dec 2021 18:21:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 14 Dec 2021 18:21:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7121d42a6972f1cbcce5d40298238b9d7b9f3322ae0dc2998efb6c7e832913`  
		Last Modified: Tue, 14 Dec 2021 18:23:23 GMT  
		Size: 6.3 MB (6252763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dca40ea6b0f35b34a260b3201f68e776570a0864f41cea6a33404e21fcbe20`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8b28333f514f833e264948ff359ae8dd3a2c8dacad7956d163b25dbecd5cd`  
		Last Modified: Tue, 14 Dec 2021 18:24:24 GMT  
		Size: 618.3 MB (618297736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0eb674025044d8d6914d9418ebff99111bd07908c909549c3f4c868ce74984`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ec5ac06458ac7d7cd7bb49c2705a53f448f10f5cecf5cc9b4c33cda0cbd13`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e050d2e5f7be287022a8f70b6633188c6c4388588a56f03790deb99e094194`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525c0205c5d17582b72d9d489411f5862afa2de165f8095c4aeab80ad1c562b`  
		Last Modified: Tue, 14 Dec 2021 18:23:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7052545fe7c7e0fc79c30dec1074f6a2a6fccb5223bbc681a9d3b44e3acd8dd`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646896311425b412d73a2437efa3f296df91a7f53d10a4a40b2b47c239f7fa07`  
		Last Modified: Tue, 14 Dec 2021 18:23:20 GMT  
		Size: 23.6 MB (23585553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44377da25a87afb3e79d307250380fb0aab61fea24b8fcc25d70f02d207c016c`  
		Last Modified: Tue, 14 Dec 2021 18:23:17 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
